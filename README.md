# NIOSH Code

## Overview
This repository contains all of the data and code used to perform the analyses discussed in the [PAPER NAME](URL). Our overarching hypothesis is to evaluate the utility of wearable sensors in modeling upper-extremity fatigue. To test our hypothesis, we present the following two case studies:
  - **Case 1: Dynamic Order-Picking Task:** Thirty-four healthy subjects performed shoulder Internal Rotation movements by keeping their elbow flexed to 90 degrees, their wrist straight, and rotating their arm inward towards the abdomen until they reached maximal exertion. Fatigue was self-reported using the Borg rating of perceived exertion. The paper can be found [here](https://www.nature.com/articles/s41597-024-03254-8).
  - **Case 2: Shoulder Internal and External Rotation Movements**

For each of those two case studies, we examine the use of three modeling approaches:  
  - **Linear and logistic regression:** We used R to run the linear regression model as well the functional regression models.
  - Several widely used **machine learning models:** We used Python and the Pycaret library to run several machine learning models. For each model generated, we create two types, *General* and *Individual*. *General* models are trained to predict the fatigue of any potential subject provided to it. This is done by providing a model all of the data from a subset of subjects as training, then data from the remaining unseen subjects as testing. *Individual* models are specialized in predicting the fatigue of one unique subject. This is done by using data from a singular subject in both the training and testing of a model. We evaluated the predictive ability of these  models both in continuous (i.e. regression applications of machine learning models) and binary (i.e. simply identifying the presence or absence of fatigue via classification-based ML models) outcomes. We present the raw notebooks in this repository. Additionally, knitted Jupyter notebooks are hosted at [src](link).
  - **Functional regression**

Further details on how the repository is organized are provided in the [repository structure](#repository-structure).



## Requirements

### R


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
│   ├── analysis/
│   │   ├── functional-regression/
│   │   │   └── **TODO**
│   │   ├── linear-regression/
│   │   │   └── **TODO**
│   │   └── machine-learning/
│   │       ├── save_models_classification.ipynb
│   │       ├── save_models_general.ipynb
│   │       └── save_models_individual.ipynb
│   ├── data/
│   └── outputs/
│       ├── csv/
│       │   ├── classification/
│       │   ├── general/
│       │   └── individual/
│       └── figures/
├── study2/
│   ├── analysis/
│   │   ├── functional-regression/
│   │   │   └── functional_regression_case3.Rmd
│   │   ├── linear-regression/
│   │   │   └── **TODO**
│   │   └── machine-learning/
│   │       ├── data_construction.ipynb
│   │       ├── save_models_classification.ipynb
│   │       ├── save_models_general.ipynb
│   │       └── save_models_individual.ipynb
│   ├── data/
│   └── outputs/
│       ├── csv/
│       │   ├── classification/
│       │   ├── general/
│       │   └── individual/
│       └── figures/
├── .gitignore
├── LICENSE
├── README.md
└── requirements.txt
```

 - [x] Restructure directories in study2
 - [x] Update the repository structure section to show the new structure
 - [ ] Get code for linear/logistic regression implementations
 - [ ] Add code to generate figures for machine learning (study1 and study2)
 - [ ] It would be nice to [add the Jupyter "buttons"](https://openincolab.com/) to run notebooks on Colab or Deepnote. 
