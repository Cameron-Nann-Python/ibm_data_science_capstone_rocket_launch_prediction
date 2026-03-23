# Machine Learning: SpaceX Falcon 9 First Stage Landing

## Overview
To predict a successful rocket launch, various machine learning algorithms were tested:
- Logistic Regression Model
- Support Vector Machines (SVM) Model
- Decision Tree Model
- KNN Model

The data used for model training comes from a previous lab: ![Python EDA](https://github.com/Cameron-Nann-Python/ibm_data_science_capstone_rocket_launch_prediction/tree/main/step_4_eda_python). Categorical features were one-hot encoded to assume a data type appropriate for modeling.

## Standarize the Data
The features were standardized using a StandardScaler() object due to the wide differences in values from different unit of measure. 

## Make Training and Test Sets
The X and Y data sets were used to make training and test sets using train_test_split(). There were only 18 classes available for training after the split, so a validation set was not made. Instead, cross-validation was implemented for model training. 

## Hyperparameter Tuning
To ensure the models select the best parameters for training, a GridSearchCV object was produced for each classification model.

### Logistic Regression 
The GridSearchCV object using a logistic regression estimator achieved an accuracy of 0.85 on the training data and 0.83 on the test data. For the 18 classes, the model successfully predicted 15 classes, but incorrectly predicted 3 as false positives.

![Logistic Regression Confusion Matrix](https://github.com/Cameron-Nann-Python/ibm_data_science_capstone_rocket_launch_prediction/blob/main/step_7_machine_learning/screenshots/logreg_conf_mat.png)

### SVM
The GridSearchCV object using an SVM estimator achieved an accuracy of 0.86 on the training data and 0.83 on the test data. For the 18 classes, the model successfully predicted 15 classes, but incorrectly 3 as false positives, similar to the logistic regression model.

![SVM Confusion Matrix](https://github.com/Cameron-Nann-Python/ibm_data_science_capstone_rocket_launch_prediction/blob/main/step_7_machine_learning/screenshots/svm_conf_mat.png)

### Decision Tree
The GridSearchCV object using a decision tree estimator achieved an accuracy of 0.93 on the training data and 0.83 on the test data. For the 18 classes, the model successfully predicted 15 classes, but incorrectly 3 as false positives, similar to the logistic regression model.

![Decision Tree Confusion Matrix](https://github.com/Cameron-Nann-Python/ibm_data_science_capstone_rocket_launch_prediction/blob/main/step_7_machine_learning/screenshots/tree_conf_mat.png)

### KNN
The GridSearchCV object using a KNN estimator achieved an accuracy of 0.93 on the training data and 0.83 on the test data. For the 18 classes, the model successfully predicted 14 classes, but incorrectly 2 as false positives and 2 as false positives.

![KNN Confusion Matrix](https://github.com/Cameron-Nann-Python/ibm_data_science_capstone_rocket_launch_prediction/blob/main/step_7_machine_learning/screenshots/knn_conf_mat.png)

## Considerations
- The decision tree model performs the best with the highest accuracy on the training and test data sets.

## Technologies Used
- Python 3.13
- Pandas, Numpy: matrix and vector array operations
- Matplotlib, Seaborn: data visualization
- Scikit-Learn: standardization and machine learning

## Import Libraries
Run the following code in a virtual environment to import libraries:
```
pip install -r requirements.txt
```

## Files Included
- `SpaceX_Machine Learning Prediction_Part_5.ipynb`: Jupyter lab notebook containing full predictive analysis provided by IBM
- `requirements.txt`: List of Python dependencies required for lab
