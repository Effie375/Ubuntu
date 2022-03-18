# Conda Cheat Sheet

Command line package and environment manager

## Conda basics

Verify conda is installed, check version number

```none
conda info
```

Update conda to the current version

```none
conda update conda
```

## Using environments

Create a new environment named myenv

```none
conda create --name myenv
```

Activate the new environment myenv to use it

```none
conda activate myenv
```

Deactivate the current environment

```none
conda deactivate
```

Get a list of all my environments, active environment is shown with *

```none
conda env list
```

List all packages and versions installed in active environment

```none
conda list
```

Install a new package (Jupyter Notebook) in the active environment

```none
conda install jupyter
```

Install a package included in Anaconda

```none
conda install spyder
```

Run an installed package (Jupyter Notebook)

```none
jupyter-notebook
```

Remove your environment

```none
conda env remove --name myenv
```

Output requirement string only

```none
conda list --export > requirements.txt
```

Install from requirements file

```none
conda install --file requirements.txt
```

To update Anaconda on Ubuntu, start by updating the `conda` utility:

```none
conda update conda
```

Next, run the Anaconda package update command:

```none
conda update anaconda
```
