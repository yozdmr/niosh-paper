# NIOSH Code (finalize this title)

## Overview
This repository contains all of the data and code used to perform the analyses discussed in the [PAPER NAME](URL). Our overarching hypothesis is to evaluate the utility of wearable sensors in modeling upper-extremity fatigue. To test our hypothesis, we present the following two case studies:
  - **Case 1: Dynamic Order-Picking Task** Short description.
  - **Case 2: Shoulder Internal and External Rotation Movements** Short description.  

For each of those two case studies, we examine the use of three modeling approaches:  
  - **Linear and logistic regression:**
  - Several widely used **machine learning models:**
  - **Functional regression:**
We utilized R and Python to run those models. Specifically, we used R to run the linear regression model as well the functional regression models. On the other hand, we used Python to run the machine learning models, evaluating the utility of those models in predicting continous fatigue outcomes (i.e., regression applications of machine learning models) and binary outcomes (i.e., the presence or absence of fatigue with classifcation machine learning-based models). We present the raw Python and RMarkdown notebooks in the folders below. Additionally, the knitted RMarkdown HTMLs and Jupyter notebooks are available at: [](), [](), ... . 

Further details on how the repository is orgainzed is provided in the [repository structure](#repository-structure).

## To do:
 - [x] Restructure directories in study2
 - [ ] Update the repository structure section to show the new structure
 - [ ] Get code for linear/logistic regression implementations
 - [ ] Write code to get figures for machine learning (study1 and study2)
 - [ ] It would be nice to [add the Jupyter "buttons"](https://openincolab.com/) to run notebooks on Colab or Deepnote. 



## Requirements

### R
TODO needs:
 - R version
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

