# Data Wrangling: SpaceX Falcon 9 First Stage Landing

## Overview

The data at this each stage needs to be explored to find trends and create labels for machine learning. The data contains successful and unsuccessful launches, which will be labeled with 1 and 0 respectively in a new column called "Class".

## Objectives

Data exploration was the first part of the data wrangling process. Missing values and data types were assessed after opening the rocket launch dataset. The first task involved finding the number of launches per launch site along with a second task of determining the number of orbit variations. 

The third exploration task was to calculate the number and occurrence of mission outcomes, which was the basis for the class column. From this observation, a set of unsuccessful outcomes was made as conditional statement for a list comprehension of class labels (see notebook). The final task was the creation of the new column from the list comprehension.

## Technologies Used
- Python 3.13
- Pandas: matrix operations
- Numpy: array operations
  
## Import Libraries
Run the following code in a virtual environment:
```
pip install -r requirements.txt
```

## Files Included
- `labs-jupyter-spacex-Data wrangling.ipynb`: capstone lab notebook for data wrangling provided by IBM
- `requirements.txt`: Python dependencies used for lab
