# Swire Coca-Cola Project

## Objective Summary
  - Swire Coca-Cola faces an issue with identifying customers, brands, and clients in their book of business to offload to White Truck services within their Western USA market. Businesses currently on Red Truck services take up a lot of resources.  Additionally, there is a need to segment and profile customers who purchase below 400 gallons per year to guide strategic outreach. Thus, we aim to identify who and who not to offload onto the White Truck services.
  - The primary objective of this project is to build a predictive and descriptive modeling framework that:
    - Identifies customer segments with consistently low ordering volumes.
    - Predicts whether a customer is likely to purchase fewer than 400 gallons in Year 2.
    - Explores operational and demographic characteristics (e.g., LMP status, CO2 status, delivery channels) to uncover behavioral patterns.
    - Supports targeted engagement strategies by clustering customers based on ordering behavior and profile.
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


