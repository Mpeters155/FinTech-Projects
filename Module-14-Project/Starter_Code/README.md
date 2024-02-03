# Machine Learning Trading Bot - Michael Peters

## Support Vector Machine
Training Period - 3 months \
Simple Moving Average - 4 days, 100 days\
Testing Report
              
              precision    recall  f1-score   support

        -1.0       0.43      0.04      0.07      1804
         1.0       0.56      0.96      0.71      2288

    accuracy                           0.55      4092
    macro avg      0.49      0.50      0.39      4092
    weighted avg   0.50      0.55      0.43      4092

### Actual Returns vs. Strategy Returns (3 month training, 4/100 day SMA)
![{Returns}](<svm_ret.png>)
#

## Support Vector Machine
Training Period - 6 months\
Simple Moving Average - 4 days, 100 days\
Testing Report

              precision    recall  f1-score   support

        -1.0       0.44      0.02      0.04      1732
         1.0       0.56      0.98      0.71      2211

    accuracy                           0.56      3943
    macro avg      0.50      0.50      0.38      3943
    weighted avg   0.51      0.56      0.42      3943

### Actual Returns vs. Strategy Returns (6 month training, 4/100 day SMA)
![{Returns}](<svm_tuned_ret.png>)
#

## Support Vector Machine
Training Period - 3 months\
Simple Moving Average - 30 days, 90 days\
Testing Report

              precision    recall  f1-score   support

        -1.0       0.43      0.44      0.44      1741
         1.0       0.56      0.55      0.55      2231

    accuracy                           0.50      3972
    macro avg      0.49      0.49      0.49      3972
    weighted avg   0.50      0.50      0.50      3972

### Actual Returns vs. Strategy Returns (3 month training, 30/90 day SMA)
![{Returns}](<svm_30_90_ret.png>)
#

## Logistic Regression Model
Training Period - 3 months\
Simple Moving Average - 4 days, 100 days\
Testing Report

              precision    recall  f1-score   support

        -1.0       0.44      0.33      0.38      1804
         1.0       0.56      0.66      0.61      2288

    accuracy                           0.52      4092
    macro avg      0.50      0.50      0.49      4092
    weighted avg   0.51      0.52      0.51      4092

### Actual Returns vs. Strategy Returns (3 month training, 4/100 day SMA)
![{Returns}](<lr_ret.png>)
#

## Conclusion
Based on the the testing reports and plots above, it seems the SVM model using 6 months of training data and the SMA's of 4 and 100 days performed the best. When changing the SMA's to 30 and 90 days the returns did the worst of any of the models.