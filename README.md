# FSM-reinforcement learning
This repository contains the code and thesis PDF file for my master's dissertation, 
named _Using deep reinforcement learning for exploring state spaces of finite state machines_.

The project experimentally uses deep reinforcement learning algorithms, namely A2C and PPO, to explore the state spaces of (possibly extremely large) finite state machines, in order to provide an easier way to validate their correctness. To ease the code development, an implementation of A2C and PPO algorithms from [Stable-Baselines3](https://stable-baselines3.readthedocs.io/en/master/) has been used, as well as the [Pydot](https://pypi.org/project/pydot/) package to render the exploration process of the algorithms.

We also experimented with the use of [Optuna](https://optuna.readthedocs.io/en/stable/) to check how hyperparameter tuning would affect the performance of the algorithms.

## Installation

Firstly, clone the repository in Git Bash using:

`git clone https://github.com/mlegas/FSM-reinforcement-learning.git`

To create a new Anaconda environment that will install the packages used in this project, use the following command in the Anaconda prompt while being inside this directory:

`conda env create -f environment.yml`

Then run the following command to activate the environment:

`conda activate FSM_RL`

In order to use the Jupyter notebooks, run the following command in the Anaconda prompt inside this directory:

`jupyter lab`

And done! A local Jupyter website should show up inside your default web browser.
If that does not happen, try to load the following website:

`http://localhost:8888/lab`

Another method is to use a Visual Studio Code IDE with the extensions for Python and Jupyter, 
which will create a local jupyter kernel that will use the conda environment.

## Usage

The main notebook for further use has been provided in the main directory, named `fsm_env.ipynb`. 

The files containing the finite state machines are located inside the `./csv_files/` directory.
The main Jupyter notebooks that were used during the development of this project
are located inside the `./evaluation_jupyter_notebooks/` directory, which can provide a further insight as to how the project works.

Additionally, the thesis has been provided as the `2031545.pdf` file.
