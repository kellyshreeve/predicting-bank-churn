# Predicting Bank Churn (Imbalanced Classifier)

<p align="center">
  <img src="https://github.com/kellyshreeve/gold-recovery/blob/main/images/recovery_process.png" 
  alt="Image of gold recovery stages">
</p>

# Project Overview

This repository hosts an Supervised Machine Learning project building a multi-output regression that minimizes symmetric Mean Absolute Error (sMAPE) when predicting gold recovery from ore. Linear Regression, Decision Tree Regression, and Random Forest Regression were tuned and cross-validated to determine which model best minimizes sMAPE on the training set. After identifying the best model, the model is used to determine which factors are unprofitable.

# Installation and Setup

## Codes and Resources Used

  - <b>Editor Used</b>: Visual Studio Code
  - <b>Python Version</b>: 3.10.9

## Python Packages Used

  - <b>General Purpose</b>: ```numpy```
  - <b>Data Manipulation</b>: ```pandas```
  - <b>Data Visualization</b>: ```matplotlib```
  - <b>Statistical Analysis</b>: ```statsmodels```
  - <b>Machine Learning</b>: ```sklearn```
    
# Data

## Source Data

### Data Files

Three data sets contain information on the full set, training set, and test set:  

*gold_recovery_full.csv*  
*gold_recovery_train.csv*  
*gole_recovery_test.csv* 

Datasets contain information on input and output measures for each stage in the gold recovery process: 

  * Inputs are floatbank parameters such as air and water level and concentrations of metal and solids in the ore.  
  * Outputs are concentrations of metals and other solids in the concentrate and in the tails.  

Observations close to each other in time are often similar.

### Feature naming construction:  

[stage]_[parameter_type].[parameter_name]

## Data Acquisition

The data were provided by TripleTen's Data Science bootcamp. As such the full dataset is loaded into the notebook but is proprietary information and cannot be shared online with the project.

## Data Preprocessing

Data were checked for missing values and duplicates. Missing values were imputed with the average of forward and backward fill. There were no duplicates.
 
# Code Structure
```
  ├── LICENSE
  ├── README.md          
  │
  ├── images
  │   └── final_regression.png
  │   └── gold_stages.png   
  │   └── recovery_process.png    
  │
  └── notebooks  
     └── gold-recovery-analysis.ipynb
 
```

# Results and Evaluation

<p align="center">
  <img src="/images/roc_auc.png" 
  alt="ROC-AUC of Test Set">
</p>


# Future Work

# Acknowledgments/References

TripleTen's Data Science bootcamp for providing the project and the data.

