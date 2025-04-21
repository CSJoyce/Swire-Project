# Swire Coca-Cola Project

## Objective Summary
  - HomeCredit Inc. aims to identify high-risk customers who are likely to default on their loans, as well as identify low-risk customers who have little to no line of credit.  The objective of this project is to construct predictive models using historical data to distinguish customers based on their ability to repay their loan.
## Solution 
  - Utilizing an XGBoost model, expanded HomeCredit's customer base to customers that were predicted to not default on loans, even with a sparse credit history.  Additionally, used a random forest model to identify customers who were at high risk for defaulting to reduce business costs.
## Personal Contribution 
  - As part of the data modeling process, I constructed a Naive Bayes classifier and LightGBM model in attempts to improve classsification performance relative to a majority-based classifier for the dataset.
      - [LightGBM Model](https://github.com/CSJoyce/CSJoyce.github.io/blob/main/hc_lightgbm.Rmd)
      - [Naive Bayes Model](https://github.com/CSJoyce/CSJoyce.github.io/blob/main/hc_naivebayes.Rmd)
## Business Value 
  - From our models, we were able to improve both the performance of the classification of low-risk, non-defaulting customers and the identification of high-risk, defaulting customers relative to the performance of majority-based classification of the data.  This allows HomeCredit Inc. to both extend loans to customers who are confidently low-risk and avoid incurring costs from defaulting by customers who are at higher likelihood to do so.
## Reflection 
  - We encountered the most difficulty in the process of exploratory data analysis.  As this was a large dataset consisting of hundreds of thousands of rows and over a hundred features, there was a large amount of missing data.  We experimented with many different techniques in the data cleaning process.  Ultimately, we decided to reduce complexity by eliminating features that contributed nothing to the predictive ability of our models, and impute data to replace missing values.  I found that training individual models took much more time than expected, and therefore the tuning and model-specific preprocessing that is done beforehand is important to evaluate before training models for hours on end to reach mediocre results or a non-functioning model.


