# CS/ME 598 SML, Spring 2026: Scientific Machine Learning

## Course info:
* Tuesdays and Thursdays, 9:30-10:45am
* Location: CIF 2036
* Instructors:
  * Prof. Luke Olson, http://lukeo.cs.illinois.edu/
  * Prof. Matt West, https://lagrange.mechse.illinois.edu/
  * <span style="color:red">Are you looking to join the class?</span>   Unfortunately the class is full!  Auditing and sitting in on the class cannot be accommodated.  Sorry! (In future semesters we are hoping to expand the offering.)

## Course links:
* Syllabus (information): https://github.com/598sml/598sml-s26-syllabus
* Syllabus through Colab: https://colab.research.google.com/github/598sml/598sml-s26-syllabus
* Github classroom (assignments): https://classroom.github.com/classrooms/254953531-598sml-s26
* Slack: https://598sml-f23.slack.com/

## Topics:

A rough outline of topics is as follows:

* What is SciML?
* Automatic Differentiation
* Approximation Theory
* SciML software
* PINNs
* PINN variants
* DeepONets
* Neural ODEs
* Closure models
* MPNNs/GNNs
* Multiscale architectures and training
* Learning solvers

## Jupyter notebooks:

There are at least three options for notebooks:

- Run locally:
  - make a virtual environment: `python -m venv ~/.venv/598sml`
  - activate it: `source ~/.venv/598sml/bin/activate`
  - install PyTorch++: `pip install torch matplotlib scipy numpy`
- iCRN @ NCSA, Illinois Computes:
  - https://jupyter.ncsa.illinois.edu/
- Google Collab
  - https://colab.research.google.com/

## Notes:

- 2026-01-20: [notes-20260126.pdf](./lectures/notes-20260126.pdf)

## Homeworks

Homework | Topic | Due date | GitHub Classroom link
--- | --- | --- | ---
HW0 | Auto diff | Thu, Jan 22 | https://classroom.github.com/a/liziYDTZ
HW1 | Numpy & Pytorch | Thu, Jan 29 | https://classroom.github.com/a/ZLiCOZ0s
HW2 | Optimization | Thu, Feb 5 | https://classroom.github.com/a/Be2iQVoq
HW3 | Function approx | Thu, Feb 12 | https://classroom.github.com/a/XYRjkVBi
HW4 | PINNs Burgers | Thu, Feb 19 | https://classroom.github.com/a/ZERchO3Y
HW5 | PINNs Poisson | Tue, Feb 24 | https://classroom.github.com/a/BT--GbtI
HW6 | DeepONets | Thu, Mar 5 | https://classroom.github.com/a/ECboR7qr
HW7 | FNOs | Thu, Mar 12 | https://classroom.github.com/a/QPgBQ6wg

## Lecture schedule:

- Week 1 (1/20)
  - What is SciML
  - [DeepMind WeatherNext 2 paper](https://arxiv.org/pdf/2506.10772)
  - [Neural GCMs paper](https://www.science.org/doi/10.1126/sciadv.adv6891)
  - [Generative downscaling paper](https://www.pnas.org/doi/10.1073/pnas.2420288122)
  - [Neural Helmhotlz inverse solver paper](https://academic.oup.com/gji/article/239/3/1469/7760394)
  - [Surrogate modeling paper](https://gmd.copernicus.org/articles/18/3681/2025/)
  - Automatic Differentiation 
  - https://jmlr.org/papers/v18/17-468.html
  - https://colah.github.io/posts/2015-08-Backprop/
  - http://neuralnetworksanddeeplearning.com/chap2.html
  - https://openreview.net/pdf?id=BJJsrmfCZ
  - https://sidsite.com/posts/autodiff/
  - https://docs.pytorch.org/tutorials/beginner/basics/autogradqs_tutorial.html
  - https://www.machinelearningexpedition.com/automatic-differentiation-in-pytorch/
- Week 2 (1/27):
  - Auto diff, [notes-20260210.pdf](./lectures/notes-20260210.pdf)
  - [Weights & Biases (W&B) guide](./lectures/wandb.md)
- Week 3 (2/03):
  - Function approximations
  - [notes-20250203-func-approx.pdf](./lectures/notes-20250203-func-approx.pdf)
- Week 4 (2/10):
  - Burgers, PINNS
  - [notes-20260210.pdf](./lectures/notes-20260210.pdf)
- Week 5 (2/17):
  - [An Expert’s Guide to Training Physics-Informed Neural Networks](https://arxiv.org/abs/2308.08468) (Wang et al., 2023)
- Week 6 (2/24):
  - Neural operators, DeepONets
  - [notes-20260224-deeponets.pdf](./lectures/20260224/notes-20260224-deeponets.pdf)
  - Notebook: [DeepONets for the derivative operator](./lectures/20260224/deeponet-derivative.ipynb)
  - DeepONet paper ([DOI:10.1038/s42256-021-00302-5](https://doi.org/10.1038/s42256-021-00302-5) or [arXiv:1910.03193](https://arxiv.org/abs/1910.03193))
- Week 7 (3/03 Tu):
  - prj00
- Week 7 (3/05 Th):
  - Fourier Neural Operators (FNOs)
  - [notes-20260305-fourier-neural-operators.pdf](./lectures/notes-20260305-fourier-neural-operators.pdf)
  - Notebook: [FNO for Poisson 1D](./lectures/20260305/FNO_Poisson1D_demo.ipynb)
  - Fourier Neural Operator paper ([ICLR 2021](https://openreview.net/forum?id=c8P9NQVtmnO) or [arXiv:2010.08895](https://arxiv.org/abs/2010.08895))
- Week 8 (3/10 Tu): prj01
  - https://github.com/598sml/prj01
- Week 8 (3/12 Th): ....
- Week 9 (3/17):  Spring Break
- Tentative:
- Week 10 (3/24 Tu): prj02 (due)
- Week 10 (3/26 Th): ...
- Week 11 (3/31 Tu): prj03
- Week 11 (4/02 Th): ...
- Week 12 (4/07 Tu): prj04
- Week 12 (4/09 Th): ...
- Week 13 (4/14 Tu): prj05
- Week 13 (4/16 Th): ...
- Week 14 (4/21 Tu): prj06
- Week 14 (4/23 Th): ...
- Week 15 (4/28 Tu): Presentations (01-10 @ 7 min) (prj07 due)
- Week 15 (4/30 Th): Presentations (11-20 @ 7 min)
- Week 16 (5/05 Tu): Presentations (21-30 @ 7 min)

## Projects


### Goals

The goal of the project is to undertake a deep dive into a specific aspect of
SciML in a direction that we have not fully covered in class.  The project must
be in SciML (for example we are not interested in generic LLMs or image
training etc) --- most often there should be a PDE or ODE or numerical
method/model driving the core exploration.

HPC, Physics, UQ, error estimation, PINN variants, turbulence, use of
transformers, GNNs, etc are all good topics.  You may (and should!) connect this
with your own research if you can.

### Guidelines

The project can be done in solo or in pairs.  If done in pairs, then you are
agreeing to equal effort on coding, writing, and presenting.

There will be regular updates (see below).  Be prepared to present updates!

A presentation will serve as the final.  The length will depend on the number of groups
but expect something in the 5-10 minute range with a specific format.

### Steps

- prj00: selecting a topic
  - `598sml/prj_topicname`
  - example: `598sml/prj_cpinn_convergence`
  - Short project description
  - Peer feedback
- prj01: description of the topic with steps
  - 0.5-1 page of details include steps
- prj02: goals and workflow
  - Identify short, medium, and stretch goals
  - Outline
- prj03: setup and initial results
- prj04: summarize model, loss, training
- prj05: peer feedback
- prj06: slides draft (1-3, specific format)
- prj07: final slides (due before first presentation)

## Course blurb

Familiarity with introductory numerical methods (e.g., CS 357 or TAM 470) and
is a prerequisite, preferably with some experience with numerical PDEs. The
course will cover the theory and practice of Scientific Machine Learning
(SciML), which leverages machine learning tools for scientific computing.
Topics include learning-based methods for differential equations, neural ODEs
and PDEs, physics-informed networks and model discovery, interpretable and
explainable learning, differentiable and probabilistic programming for
scientific computing, and uncertainty quantification via learning. Efficient
parallel implementation of algorithms on scalable computing architectures will
be emphasized.

## What to expect

The course requires some background in numerical methods (e.g. CS357, CS450, or
TAM 470 type courses), but no prior knowledge of machine learning or experience
with neural networks.  As such, the course will build the necessary tools through
the semester, with a focus on scientific applications.

The course is project based, particularly the last half.  You will use `git`,
`pytorch`, and `latex` to develop various examples and steps toward your final
project.

Assignments will be submitted on Github Classroom at  https://classroom.github.com/classrooms/254953531-598sml-s26

## Grading

Final course scores will be computed as 40% Homeworks and 60% Final Project.

## Attendance and Illness

Class attendance is expected, however...

If you have any cold-like symptoms or do not feel well, then you should not
attend class, regardless of testing negative or positive for COVID.

Your missed attendance due to illness will not impact
your grade in the course and we will work with you keep you up-to-date
on the material.
