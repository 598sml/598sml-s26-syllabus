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
- Week 4 (2/10):
  - Burgers, PINNS
  - [notes-20260210.pdf](./lectures/notes-20260210.pdf)
- Week 5 (2/17):
- Week 6 (2/24):
- Week 7 (3/03):
- Week 8 (3/10):
- Week 9 (3/17):  Spring Break
- Week 10 (3/24): ...
- Week 11 (3/26): ...

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
