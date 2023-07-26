# Fraud
## I'll walk you through each stage for what I done, while giving a general overview:
### Data preprocessing: 
The first step is to search the dataset for missing values and outliers. There are no missing values discovered, and the quantile approach is used to handle outliers.
### Data visualisation: 
To comprehend the distribution and find potential insights, the data is displayed using histograms and box plots.
### Encoding: 
To make categorical variables like "type," "nameOrig," and "nameDest" into numeric forms for modelling, they are label-encoded.
### Correlation:
Heatmaps are created to check for multicollinearity between features during the multicollinearity check process. Features that are highly linked are found and removed from the dataset.
### Model Building:
The dataset is divided into training and testing sets for model building. A fraud detection model is constructed using XGBoost, and feature selection is carried out using XGBoost's feature significance.
### RandomizedSearchCV :
is used to fine-tune the hyperparameters of the Random Forest classifier.
### Evaluation of the Model: 
The accuracy, precision, recall, F1-score, and ROC AUC metrics are used to assess the performance of the final fraud detection model.
#### Final result: 
- Accuracy: 0.9996479437715909
- Precision: 0.9614173228346456
- Recall: 0.7537037037037037
- F1-Score: 0.8449826989619377
- ROC AUC: 0.8768325742352892
- Confusion Matrix:
 [[1270855      49]
 [    399    1221]]
