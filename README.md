## Credit-Risk

Using algorithms - 
1. Logistic Regression
2. KNeighborsClassifier
3. DecisionTreeClassifier
4. SVC
5. RandomForestClassifier
6. XGBClassifier  

(while dealing with Feature Engineering, Imbalance in Dataset) to classify if an individual would subject to Credit Risk with the given data - age, income, home ownership, loan intent, loan interest rate etc. 

## Description
- Downloaded from Kaggle, this dataset is medium in size - with 32581 rows and 12 columns.
- This dataset was selected to showcase the concepts of RandomizedSearchCV with multiple classifiers, How to deal with Imbalance in Target Variable and how sticking to the basics can transform the model to outperform expectations.

## Workflow 

```mermaid
flowchart LR
  A[Install and Imports] --> B[Loading the Dataset]
  B --> C[EDA and Data Cleaning]
  C --> D[Modeling]
  D --> E[Resampling the Data]
  E --> F[Inference]
```

## Inference

- After the initial run of model training, validations resulted in proving that DecisionTree, SVC, RandomForest as the better performing models.
- Overfitting wasn't hueg as seen by error plots, but still prevalent. 
- Analysis revealed imabalance of target variable in the dataset affected the model performance.
- A combination of Majority and Minority Sampling resulted in the significant reduction in overfitting.
- Exchanging the model accuracy for precision-recall is a good call when it comes to imbalanced classification.

