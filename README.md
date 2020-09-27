# Credit_Risk_Challenge

### Resampling Model Results

For Oversampling, I ran two methods of analysis. For Naive Random Oversampling, the dataset is resampled so we can train a model, make predictions, and evaluate the performance. The balanced accuracy score for this model was 68%. However, this number can be misleading. Examining the classification report, the average precision score is 99%, an average recall score of 63% and an F1 score of 77%.

Using the SMOTE Overampling method, the balanced accuracy score remains the same at 68%. Per the classification report, the average precision score is 99%, recall score of 68% and F1 score of 81%.

For Undersampling, after running the Cluster Centroids algorithm the balanced accuracy score was 65%. The average precision score is 99%, average recall is 41% with a F1 score of 58%.

For Combination, I resampled the data using SMOTEENN algorithm which combines aspects of both oversampling and undersampling. The accuracy score was 55%, with an average precision score of 99%, average recall of 59% and F1 score of 74%.

### Resampling Conclusion and Recommendation

My recommendation for this data set would be to use the SMOTE Oversampling method, as it has a high F1 score of 81% and has the highest balanced accuracy score of 68% compared to the other models. The F1 score is defined as the mean between precision and recall and is used as the statistical measure to rate performance of a particular test.

### Ensemble Model Results

After running the Ensemble Models, the Balanced Random Forest Classifier returned a balanced accuracy score of 79%, an average precision score of 99%, recall score of 87% and F1 score of 93%. When the features were sorted the total_rec_prncp and total_pymnt were the most important. By using the Easy Ensemble Classifier model, the balanced accuracy score was 93%, with a precision score of 99%, recall score of 94% and F1 score of 97%.

### Ensemble Conclusion and Recommendation

The Easy Ensemble Classifier Model returned high values for each statistic - balanced accuracy score, precision, recall and F1 were all in the 90th percentile. I would recommend using this test to predict credit risk. The Easy Ensemble Classifier is a bag of balance boosted learners.
