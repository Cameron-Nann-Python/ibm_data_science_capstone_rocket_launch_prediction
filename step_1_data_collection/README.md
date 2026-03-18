# Data Collection: SpaceX Falcon 9 First Stage Landing

## Overview
The object of this capstone project is to predict if the Falcon 9 first stage will be successful. SpaceX has rocket launches that cost less than those of its competitors due to the first stage being reusable. This stage in the lab will collect and clean data from an independent API that collects rocket launch data from SpaceX.

## Objectives
The first part of the data collection process will to be obtain data from a SpaceX API (provided by r/SpaceX API Docs). A series of helper functions will read the data from the API into lists (columns) that will be stored in a dictionary. The dictionary will then be converted into a pandas DataFrame. 

The second part of the data collection process will to be clean the data. Missing values will be imputed with the mean and dates will be converted into readable formats. Columns irrelevant to the Falcon 9 will be dropped from the data frame. The final data frame will be saved as a csv for portability.

## Technologies Used
Python libraries
- `requests`: used to make HTTP requests to obtain data from the API as a .json response.
- `pandas (3.0.1)`: used to store data into a dataframe for easy manipulation
- `numpy (2.4.2)`: used for array/matrix operations
- `datetime`: used for date format conversions

## Import Libraries
Run the following code in a virtual environment:
```
pip install -r requirements.txt
```

## Files Included
- `jupyter-labs-spacex-data-collection-api.ipynb`: capstone lab notebook for data collection provided by IBM.
- `jupyter-labs-webscraping.ipynb`: capstone lab notebook for webscraping launch data on wikipedia provided by IBM.
