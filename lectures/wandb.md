# CS/ME 598 Weights & Biases (W&B) Setup Guide

This guide explains the **minimal configuration** needed to use **Weights & Biases (W&B)** for experiment tracking in CS/ME 598 SML across:

- Local laptops
- Google Colab
- UIUC ICRN cluster

The goal is: **easy setup, no ops burden, portable skills, and reproducible experiments**.

---

## 0. Create a W&B account (once)

1. Go to https://wandb.ai
2. Sign up using your **illinois.edu email**
3. Go to **Settings → API Keys**
4. Copy your API key (you will use it below)

⚠️ Never commit your API key to GitHub.

---

## 1. Install W&B

### Local laptop or ICRN
```bash
pip install wandb
```

### Google Colab
```python
!pip install wandb
```

---

## 2. Authenticate (once per environment)

### Recommended (interactive)
```bash
wandb login
```
Paste your API key when prompted.

### Alternative (batch / non-interactive)
```bash
export WANDB_API_KEY=your_api_key_here
```

---

## 3. Environment-specific configuration

### A. Local laptop

Before running training:
```bash
export WANDB_PROJECT=598-sml
export WANDB_DIR=./wandb
```

Notes:
- Logs are stored locally in `./wandb`
- Works well for laptops and local virtual environments

---

### B. UIUC ICRN cluster (recommended setup)

Before running training:
```bash
export WANDB_PROJECT=598-sml
export WANDB_DIR=$SCRATCH/wandb
```

Why this matters:
- Avoids writing to `$HOME`
- Prevents shared filesystem slowdowns
- Keeps logs user-isolated

If running batch jobs, set these in your job script.

---

### C. Google Colab

No special configuration required.

Recommended first cell:
```python
import wandb
wandb.login()
```

Colab handles filesystem and networking automatically.

---

## 4. Minimal Python usage (required)

```python
import wandb

wandb.init(
    project="598-sml",
    name=f"{model_name}-seed{seed}",
    config={
        "lr": 1e-3,
        "batch_size": 64,
        "model": model_name,
        "seed": seed,
    }
)

for epoch in range(num_epochs):
    train_loss = ...
    val_loss = ...

    wandb.log({
        "epoch": epoch,
        "train_loss": train_loss,
        "val_loss": val_loss,
    })

wandb.finish()
```

That is all that is required.

---

## 5. What to log (and what NOT to log)

### ✅ Log
- Scalar metrics (loss, accuracy, etc.)
- Hyperparameters / config
- Small plots or tables
- **Optional:** best model checkpoint only

### ❌ Do NOT log
- Datasets
- API keys or `.env` files
- Full checkpoint sweeps
- Anything private or sensitive

Think of W&B as a **lab notebook**, not a data lake.

---

## 6. Offline mode (fallback)

If networking fails (rare but possible on clusters):

```bash
export WANDB_MODE=offline
```

Later, sync from a login node or laptop:
```bash
wandb sync /path/to/wandb/run-*
```

---

## 7. Local backups

In addition to W&B, you should save locally:
- `metrics.csv`
- `config.yaml` or `config.json`
- Git commit hash (in README or report)

These ensure reproducibility.

---

## 8. Pair projects

For pair projects:
- Either share a single W&B project
- Or keep separate projects and link to both

No special permissions are required.

---

## One-sentence rule

> Log metrics and configs only, keep local backups, and treat W&B like a lab notebook.

