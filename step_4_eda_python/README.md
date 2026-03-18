# Python EDA: SpaceX Falcon 9 First Stage Landing

## Overview
To create features ready for machine learning, the dataset will need to be explored to find and transform relevant features that can predict a successful rocket launch.

## EDA Objectives
The following tasks outline the procwss for determining features relevant to successful launches:
-  Determine the relationship between flight number and launch site.
-  Determine the relationship between payload mass and launch site.
-  Determine the relationship between success rate and orbit type.
-  Determine the relationship between flight number and orbit type.
-  Determine the relationship between payload mass and orbit type.
-  Determine the relationship between launch year and success rate.

## Analysis
- Larger flight numbers have larger success rates than smaller ones.
- Successful launches appear to stop at certain payload thresholds. It can be seen that rockets launched by VAFB-SLC 4E have payloads that do not exceed 10,000 kg.
- ES-L1, GEO, HEO, and SSO are tied for the highest success rate and SO has the lowest success rate. Launches seem to struggle with medium and low orbit paths.
- For lower earth orbit (LEO), success is related to larger flight numbers. There is no relation for GTO orbits, but other orbit types show a similar relation for success.
- ISS, PO, and VLEO are orbit types that have higher success rates when payload increases. GTO does not show a significant relation.
- Launch rate success increases with a dip in 2018 and until 2020 (most likely influenced by external factors).

## Feature Engineering
The dataset was reduced to include relevant features for model training. Categorical features were transformed with one-hot encoding and the data frame was cast to float64 for machine learning.

## Technologies Used
- Python 3.13
  
## Import Libraries
Run the following code in a virtual environment:
```
pip install -r requirements.txt
```

## Files Included
- `edadataviz.ipynb`: capstone notebook for EDA and feature engineering with Python provided by IBM
- `requirements.txt`: list of Python dependenices
