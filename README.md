# Credit Risk Classification
## Description
This project aims to use various machine learning techniques to train and evaluate the performance of Logistic Regression Models in identifying the creditworthiness of borrowers. The models were trained using different methods, and their performances were compared to determine which model has better performance. The predictive variables in the model are the labels 0 (healthy loan) and 1 (high-risk loan).
## Steps
The dataset was split into features and labels, and further divided into training and testing sets.

•	Machine Learning Model 1 was built with a logistic regression model and training with the original training sets (x_train, y_train), fitting it to the training sets, and using it to generate predictions.

•	Machine Learning Model 2 was built by resampling the original training data using the RandomOverSampler module, using a logistic regression model and fitting the resampled training sets (x_resample, y_resample) to the model, and generating predictions.

The performance of each model was evaluated based on the balance accuracy score, the confusion matrix, as well as the precision score, recall score, and f1-score in the classification report.
## Results
•	Machine Learning Model 1 – Original Data
Model 1 gives an accuracy of 94.4% in predicting the 2 labels. The model is good at predicting the healthy loans, with both precision and recall scores of 1.00. However, the model's performance in predicting the high-risk loans can be improved. The precision score for high-risk loans is 0.87, indicating that only 87% of actual high-risk loans were correctly predicted. The recall score for high-risk loans is 0.89, indicating that the model only identified 89% of all high-risk loans in the dataset.

•	Machine Learning Model 2 – Resampled Data
Model 2 has an accuracy of 99.6% in predicting the 2 labels. The model is good at predicting the healthy loans, with both precision and recall scores of 1.00. The precision score for high-risk loans remains at 0.87, but the recall score has improved to 1.00, indicating that the model can now predict all high-risk loans in the dataset.

## Summary
Model 2 outperforms Model 1 in predicting high-risk loans and has an overall higher accuracy in predicting both labels. Specifically, Model 2 achieved a relatively high precision in predicting high-risk loans while correctly identifying all high-risk loans in the dataset, which is considered fairly good performance in this context. Therefore, I would recommend using Model 2 because it is better at identifying high-risk loans and has better accuracy in predicting labels.
