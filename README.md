# Liesel at the Statistics Retreat 2025

This repository contains additional materials for the Liesel session at the retreat of the chair of statistics 2025.


<img src="https://raw.githubusercontent.com/liesel-devs/liesel/main/misc/logo/logo-light.png#gh-light-mode-only" alt="logo" align="right" width="185">
<img src="https://raw.githubusercontent.com/liesel-devs/liesel/main/misc/logo/logo-dark.png#gh-dark-mode-only" alt="logo" align="right" width="185">


### Resources

- [Paper on arXiv](https://arxiv.org/abs/2209.10975)
- [Liesel & Goose repo](https://github.com/liesel-devs/liesel)
- [Liesel & Goose API docs](https://docs.liesel-project.org)
- [Liesel-GAM](https://github.com/liesel-devs/liesel_gam)


## Setup

To run the notebooks, you need the following available:

1. A working installation of Python 3.13 or newer
2. A Python environment, ideally a virtual environment, with the following packages installed:
    - `liesel` development version from the current GitHub main branch
    - `ipykernel` (for running a jupyter notebook)
    - `jupyter` (for running a jupyter notebook)

Sometimes the installation of Jax, a key dependency of both liesel and liesel_ptm is
tricky. For help, consider: https://docs.jax.dev/en/latest/installation.html

### MacOS Setup

#### Python 3.13

To check you Python version, run the follwing in a terminal:

```
python3.13 --version
```

If that fails, install via Python 3.13 via Homebrew (see https://brew.sh):

```
brew install python@3.13
```

Then verify success by running:

```
python3.13 --version
```

#### Virtual Environment Setup


First, make sure the working directory is the project directory:

```
pwd # prints working directory
```

If that is not the case, change to the project directory

```
cd /path/to/statistics-retreat-2025
```

Now initialize a new virtual environment:

```
python3.13 -m venv .venv
```

Now activate the virtual environment:

```
source .venv/bin/activate
```


#### Install packages

Now install the required packages via:

```
pip install git+https://github.com/liesel-devs/liesel.git
pip install ipykernel jupyter
```

#### Launch Jupyter Notebook

Now you can launch the demo notebooks:

```
jupyter notebook notebooks/<name.ipynb>
```


### Windows Setup

#### Python 3.13

To check your Python version, open **Command Prompt (cmd.exe)** or **PowerShell** and run:

```
py -3.13 --version
```

If that fails, try:

```
python --version
```

If neither works, download and install Python 3.13 from [python.org](https://www.python.org/downloads/).  
During installation, make sure to check:
- Add python.exe to PATH
- Install py launcher

Then verify success by running again:

```
py -3.13 --version
```


#### Virtual Environment Setup

First, make sure you are in the project directory:

```
cd path\to\statistics-retreat-2025
```

Now initialize a new virtual environment:

```
py -3.13 -m venv .venv
```

Now activate the virtual environment:

```
.venv\Scripts\activate
```

If successful, your prompt will change and show something like:

```
(.venv) C:\path\to\statistics-retreat-2025>
```


#### Install packages

Now install the required packages:

```
pip install git+https://github.com/liesel-devs/liesel.git
pip install ipykernel jupyter
```


#### Launch Jupyter Notebook

Now you can launch the demo notebooks:

```
jupyter notebook notebooks/<name.ipynb>
```
