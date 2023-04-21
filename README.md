# Git-and-GitHub-final-assignment
This template repository hosts the final Git & GitHub assignment.

## Description
We learnt how to use Git & GitHub to keep records of milestones during  projects. Now, this is time for the final assignment that consists in creating *3 repositories* each having a *minimum of 3 commits* to host some of the previous projects you worked on, during the previous phase of the program and fill the table in the `Recap Table` section.

## Assignment
The following steps constitute your assignment :
1. **Clone this repository** on your local machine; 
1. Configure it as described in the `Setup` section;
1. Select `3` projects, your own ones or projects done during the previous part of the Azubi program ;
1. **Create one public repository** for each project, with a complete and personalized readme file and repository's description ;
1. **Commit** `at least 3 times for each repository` while including simple and clear commit's messages, and **push**;
1. **Fill** the table in the `Recap Table` section with the details of your created repositories.
1. Finally, **commit** with the message `My 3 repositories has been created`, then **push your commit**.

## Recap Table
The below table must contain the details of the repositories you will create, fill it please.


|  | Project's Name | Description    | GitHub's Link  |
|:--:|:--------------:|:--------------:|:--------------:|
| 1 |  Simple Mortgage Calculator |  This is a simple Python mortgage calculator that calculates the monthly repayment and total amount paid over the life of a mortgage loan. | https://github.com/rasmodev/Simple-Mortgage-Calculator/blob/main/README.md |
| 2 |  NYC Parking Violations EDA |  This repository contains an Exploratory Data Analysis (EDA) of over 12 million records of parking violations in New York City from July 2020 to June 2021. The analysis explores the distribution of violations by state, top vehicle makes, and peak violation months and days, and provides recommendations for NYC. | https://github.com/rasmodev/NYC-Parking-Violations-EDA/blob/main/README.md |
| 3 |  House Price Prediction - California Housing Dataset |  This repository contains a machine learning algorithm that trains a model to predict house prices based on specified features of the homes, using the California Housing Dataset. The dataset used to train and evaluate a Stochastic Gradient Descent (SGD) model to predict median housing prices. The SGD model is trained using cross-validation and hyperparameter tuning to optimize its performance. The best model is then evaluated on the test set to assess its performance. | https://github.com/rasmodev/House-Price-Prediction---California-Housing-Dataset/blob/main/README.md |


**NB**: `Do not modify` the general structure of this table above to avoid issue of evaluation, just fill the rows .

## Setup
Install the required packages to be able to run the evaluation locally.

You need to have [`Python 3`](https://www.python.org/) on your system (**a Python version lower than 3.10**). Then you can clone this repo and being at the repo's `root :: repository_name> ...`  follow the steps below:


- Windows *(Python should be added to the Path variable of environment)*:
        
        python3 -m venv venv; venv\Scripts\activate; python -m pip install --upgrade pip; python -m pip install -r requirements.txt  

- Linux & MacOs:
        
        python3 -m venv venv; source venv/bin/activate; python -m pip install --upgrade pip; python -m pip install -r requirements.txt

The both long command-lines have a same structure, they pipe multiple commands using the symbol **;** but you may manually execute them one after another.

1. **Create the Python's virtual environment** that isolates the required libraries of the project to avoid conflicts;
2. **Activate the Python's virtual environment** so that the Python kernel & libraries will be those of the isolated environment;
3. **Upgrade Pip, the installed libraries/packages manager** to have the up-to-date version that will work correctly;
4. **Install the required libraries/packages** listed in the `requirements.txt` file so that it will be allow to import them into the python's scripts and notebooks without any issue.

## Evaluation
This evaluation will be automatically grade, so please follow the instructions carefully. 

You can run this command bellow being at the root of the repository to be sure your solutions are the good ones before to push your solutions.
```command
python -m pytest -v
```

If everything is okay, you will have such an output

```terminal
================================================= test session starts =================================================
platform xxx -- Python 3.9.6, pytest-7.2.0, pluggy-1.0.0 -- /xxx/python3
cachedir: .pytest_cache
rootdir: xxx/Git-and-GitHub-final-assignment
collected 3 items                                                                                                     

tests/test_filled_table.py::test_not_empty_table PASSED                                                         [ 33%]
tests/test_filled_table.py::test_not_empty_rows PASSED                                                          [ 66%]
tests/test_readme_table.py::test_contains_table PASSED                                                          [100%]

================================================== 3 passed in 0.000s ==================================================

```
