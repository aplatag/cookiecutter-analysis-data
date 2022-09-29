# Template for data analysis based on Cookicutter


## Installation modes:

1. Full:
  - It has all the libraries of basic and minimal 
  - keras
  - tensorflow
  - seaborn
  - scikit-learn

2. Basic: 
  - It has all the libraries of minimal
  - spyder
  - numba
  - opencv
  - scipy
  
3. Minimal:
  - numpy
  - matplotlib  
  - pandas
  - jupyter
  - pip

## Requirements

- Conda

## Installation of Cookiecutter
1. Create an environment

```bash
conda create -n name-environment
```
2. Install Cookiecutter

```bash
conda install -c conda-forge cookiecutter
```

## Create a new project

1. Open the environment where you have downloaded the cookiecutter package
2. Then create the project from the github repository

```bash
cookiecutter https://github.com/aplatag/cookiecutter-analysis-data
```

## Steps to finish configuring your work environment
1. Create the virtual environment of the project
```bash
  conda env create --file environment.yml
```
2. Activate the project environment
```bash
  conda activate name_project
```
3. Install project packages 
```bash
  pip install --editable .
```


## Project Organization

    ├── README.md          <- Project description.
    ├── data
    │   ├── ready_to_use   <- Data ready to use in the project.
    │   └── raw            <- Original data.
    │
    ├── scripts            <- Project script.
    │
    ├── reports  
    │   ├── results        <- Results of the project.             
    │   └── figures        <- Save high quality figures.
    │
    ├── environment.yml    <- The requirements file.
    │
    └── modules             
        ├── __init__.py    <- Python module.
        │
        ├── preprocessing           
        │   └── make_processing.py  <- Data is processed
        │
        ├── methods           
        |   └── methods.py  <- functions or methods used in the project
        │
        ├── visualization      
        │   └── display.py   <- Function to display data.
        │
        └── utils          
            └── paths.py   <- relative paths.