# NIOSH Code (finalize this title)

## Overview
This repository contains all of the code used to perform the analyses discussed in the [PAPER NAME](URL). Further details on how the repository is orgainzed is provided in the [repository structure](#repository-structure).

## Requirements

### RStudio
TODO needs:
 - RStudio version
 - Libraries used


### Python
Python is necessary for the machine learning analysis of this paper. We use [Python v3.9](https://www.python.org/downloads/release/python-3910/). A virtual environment is recommended before installing the libraries necessary for this project.

Python libraries to install:
```
pip install pycaret[full]
```

The `requirements.txt` file is also provided, however installing the libraries directly can potentially help avoid OS or version based issues when setting up the libraries on a new machine.


## Repository Structure 

The code in the repository is organized in the following folder structure:

```
niosh-paper/
├── study1/
│   ├── functional-regression/
│   ├── linear-regression/
│   └── machine-learning
│   │   ├── data/
│   │   ├── outputs/
│   │   ├── data_construction.ipynb
│   │   ├── save_models_classification.ipynb
│   │   ├── save_models_general.ipynb
│   │   └── save_models_individual.ipynb
├── study2/
│   ├── functional-regression/
│   │   └── functional_regression_case3.Rmd
│   ├── linear-regression/
│   │   └── **TODO**
│   ├── machine-learning
│   │   ├── data/
│   │   ├── outputs/
│   │   ├── data_construction.ipynb
│   │   ├── save_models_classification.ipynb
│   │   ├── save_models_general.ipynb
│   │   └── save_models_individual.ipynb
├── .gitignore
├── LICENSE
├── README.md
└── requirements.txt
```

## Further description to come...

