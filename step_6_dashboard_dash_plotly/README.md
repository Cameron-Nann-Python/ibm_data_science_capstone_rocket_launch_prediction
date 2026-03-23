# Plotly Dash Rocket Launch Dashboard: SpaceX Falcon 9 First Stage Landing

![Overall Dashboard](https://github.com/Cameron-Nann-Python/ibm_data_science_capstone_rocket_launch_prediction/blob/main/step_6_dashboard_dash_plotly/screenshots/dashboard_desktop.png)

## Overview
To gain a better understanding of launch site and booster version category on rocket launch success, a dashboard was visualizing these features was created using Dash. 

## App Layout
The app is comprised of the following features:
- app title
- dropdown for all launch sites with individual selection
- pie chart showing number of success for all sites or success rate for a single site
- slider for payload mass (kg)

## App Callbacks
- the pie chart and scatter chart slice to a specific launch site or show data for all launch sites based on dropdown input
- the scatter chart shows launch outcomes by booster version category for a selected range input

## Observations
- KSC LC-39A has the largest number of successful launches
- CCAFS SLC-40 has the higest launch success rate at 42.9%
- The FT booster version category has the highest launch sucess rate

## Technologies Used
- Python 3.13
- Dash: UI components
- Plotly: graph components

## Import Libraries
Run the following in a virtual environment:
```
pip install -r requirements.txt
```

## Files Included
- `rocket_dashboard.py`: Python file containing full dashboard logic
- `requirements.txt`: list of Python dependencies
- screenshots: folder of dashboard screenshots
