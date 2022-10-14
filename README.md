# Q-SITE 2022: Covalent QML Tutorial

<div align="center">

<img src="https://raw.githubusercontent.com/AgnostiqHQ/covalent/master/doc/source/_static/covalent_readme_banner.svg" width=150%>

</div>

This repository contains all the material needed to complete the `covalent` tutorial and challenge exercises presented at *Q-SITE 2022* (University of Toronto).

Here, you'll find:

1. The slides from the talk (`slides.pdf`).

2. Jupyter notebooks containing the tutorial (`tutorial/qsvm_tutorial.ipynb`) and challenge (`exercise/qsvm_challenge.ipynb`) scripts.

## Install instructions

To run the jupyter notebooks, you will need a Python (`conda`) environment with the requisite dependencies.

* First, clone or download this repository to your local machine.

* If you don't already have conda, navigate to [the conda download page](https://conda.io/projects/conda/en/latest/user-guide/install/download.html) and install a version of either Miniconda or Anaconda compatible with your OS. This is strongly recommended over using the 'system' Python.

* To create a fresh conda environment, navigate to root directory of this repo (`tutorials_covalent_qsite_2022`) and run

        > conda env create -f environment.yml

    This will create an environment called `qsite_covalent`.
    
* To use this environment, activate it with the following command:

        > conda activate qsite_covalent

* You can make the environment visible to your Jupyter Notebook viewer by running

        > python -m ipykernel install --user --name=qsite_covalent

    Jupyter notebooks can be opened with

        > jupyter notebook <insert-notebook-filename-or-directory>

    With the notebook open in a browser window, select the kernel (i.e. Python environment) from the 'Kernel' drop-down menu:
    
    > Kernel > change kernel > select qsite_covalent

Alternatively, you can skip the `ipykernel install` command by opening notebooks with the `qsite_covalent` environment already activated. You'll have to do this every time, so the above method is perhaps more convenient.


## Start Covalent

After successfully creating the conda environment, the Covalent server can be started as follows

        > covalent start --ignore-migrations

Covalent can optionally be started in debug mode for more verbose logging as follows

        > covalent start -d --ignore-migrations

That's it, you are good to go!
