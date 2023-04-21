# Online payments fraud detection

This is a project from the machine learning I class, using this [dataset](https://www.kaggle.com/datasets/rupakroy/online-payments-fraud-detection-dataset)

## Project goal

The problem is interesting due to class imbalance, in this case let's say we have 2 million entries, where 98% are legit transactions, and 2% are frauds, this means that we have a class imabalance problem, if a model is trained with imbalanced data, it will not perform well, as it will have a bias towards the majority class.

To solve this problem we can use either undersample or oversampling, this techniques makes models more responsive to class imbalance.

## Models used

- Logistic Regression

- Decision Trees

- Random Forest

## Results 

All models were trained with imbalanced, undersampled, and oversampled data to view the impact of these techniques, see the following table:

|  Model | recall  | ROC  | precision-Recall  |    false positives  |   true positives  |    
|---|---|---|---|---|---|
| Imbalanced Logistic Regression | 0.56  |  0.7791 | 0.7626   |   4  |   115 | 
| Undersampled Logistic Regression    |   0.99| 0.9714  | 0.5083   |  7545   |  204|  
| Oversampled Logistic Regression    |   0.99| 0.9742  | 0.5094   |   5891   |   203  |  
| Imbalanced Decision Tree  | 0.54  | 0.7278  | 0.2739  |  13236  |  111 |318.
|Undersampled Decision Tree    |   1.00| 0.9696  | 0.5089  |   8886  |   205 | 0.
|Oversampled Decision Tree    |   0.99| 0.9642   |  0.5037 |   9071   |   203  |  
| Imbalanced Random Forest  | 0.61  |  0.8058  |  0.8021   |  1  |   126  |  
| Undersampled Random Forest    | 0.7| 0.851  | 0.5188  |   290   |   145  | 
|Oversampled Random Forest    |   0.57| 0.784  | 0.7759  |   2 |   117  |  