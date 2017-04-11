# Continuously tempered Hamiltonian Monte Carlo

Python code accompanying the paper [Continuously tempered Hamiltonian Monte Carlo](http://arxiv.org).

## Installation

Two Python dependencies for running the experiment are included as submodules so you will need to do a recursive clone e.g.

```
git clone --recursive https://github.com/matt-graham/continuously-tempered-hmc.git
```

The code has only been tested with Python 2.7. The [environment.yml](environment.yml) file specifies the requirements for a [Conda](https://conda.io/docs/) environment that should be able to run all the experiments. After you have cloned the repository, from within the repository directory run

```
conda env create -f environment.yml
```

to create a new Conda environment called `cthmc` in which all the external dependencies will be installed to.

Once the `cthmc` environment is set up, activate it using

```
source activate cthmc
```

and then install the two internal Python dependencies by running

```
python thermodynamic-monte-carlo/setup.py install
python boltzmann-machine-tools/setup.py install -use-openmp
```
