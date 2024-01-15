# Module 12 Credit Risk Analysis

## Overview of the Analysis


* The purpose of this analysis is to try and accruately predict whether a loan can be made in good faith, based on borrower information.

* The data reported by the company was the loan size and interest rate, the borrower's income, their debt to income ratio, the number of accounts held, number of derogatory marks, and their total amount of debt.

* The variable we are trying to predict is whether or not the borrower is in good standing on their loan.

* For the analysis i first had to seperate the data inot the "features" (data used to make the predictions), and the "target" in this case the loan status(what we are trying to predict). 

* In this analysis I tested 2 types of Logistic Regression. 1 model i used the unaltered data, in the other I used the data that i had ran through the Random Over Sampler. 

## Results

* Machine Learning Model 1: Unaltered Dataset
  * Description of Model 1 Accuracy, Precision, and Recall scores.
      * Accuracy Score : %95.2
      * Precision
        + %100 good loan status
        + %85 bad loan status
      
      * Recall
        + %99 good loan status
        + %91 bad loan status




* Machine Learning Model 2: Random Over Sampled Dataset
  * Description of Model 2 Accuracy, Precision, and Recall scores.
    * 
      * Accuracy Score : %99.3
      * Precision
        + %100 good loan status
        + %84 bad loan status
      
      * Recall
        + %99 good loan status
        + %99 bad loan status
## Summary

* Which one seems to perform best? How do you know it performs best?
  + I believe the over sampled model performed better based on the accuracy score and the recall score.
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
  + In my opinion it would be better to have  lower false positves cases so the compnay is not giving loans to borrowers that have a greater chance of defaulting on their loan. I believe the small hit taken to false negatives would be worth the trade off in this case.