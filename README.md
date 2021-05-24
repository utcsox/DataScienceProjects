# Data Science Projects

## Installation
### 1. Check out the repo

```
git clone https://github.com/utcsox/DataScienceProjects.git
cd DataScienceProjects
```

### 2. Set up the Python environment

We use `conda` for managing Python and CUDA versions, and `pip-tools` for managing Python package dependencies.

run `make conda-update` to create an environment called `DataScienceProjects`, as defined in `environment.yml`.
This environment will provide us with the right Python version as well as the CUDA and CUDNN libraries.

Next, activate the conda environment.

```sh
conda activate DataScienceProjects
```

#### Next: install Python packages

Next, install all necessary Python packages by running `make pip-tools`

#### Set PYTHONPATH

Last, run `export PYTHONPATH=.` before executing any commands later on, or you will get errors like `ModuleNotFoundError: No module named 'DataScienceProjects'`.

In order to not have to set `PYTHONPATH` in every terminal you open, just add that line as the last line of the `~/.bashrc` file using a text editor of your choice (e.g. `nano ~/.bashrc`)
