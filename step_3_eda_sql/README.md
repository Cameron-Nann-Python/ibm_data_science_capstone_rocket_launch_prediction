# SQL EDA: SpaceX Falcon 9 First Stage Landing

## Overview
In order to determine the cost of a successful rocket launch, the payload of previous launches must be analyzed. By leveraging the power of sqllite, a database connection to the rocket launch data can be formed where queries explore various data features.

## Objectives
The following tasks describe the exploration of the dataset with sql queries:
- Identify the names of each launch site
- Preview launch site data where the launch site starts with "CCA"
- Identify the total payload mass for boosters launched by NASA (CRS)
- Identify the average payload mass for booster version F9 v1.1
- Identify the date of the first successful landing outcome in ground pad
- Identify boosters with successful drop ship landing outcomes and payload masses between 4000 and 6000 kg
- Identify total successful and failure mission outcomes
- Identify booster versions that carry the maximum payload
- Show failures in 2015
- Show number of landing outcomes from 2010-06-04 to 2017-03-20

## Technologies Used
- Python 3.13

## Import Libraries
Run the following code in a virtual environment:
```
pip install -r requirements.txt
```

## Files Included
- `jupyter-labs-eda-sql-coursera_sqllite.ipynb`: capstone notebook for EDA with SQL provided by IBM
- `requirements.txt`: list of Python dependencies used for lab.
