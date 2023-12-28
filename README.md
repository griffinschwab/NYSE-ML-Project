# New York Stock Exchange Machine Learning Project
This is a machine learning project using New York Stock Exchange data.

## Clean and Wrangle the Data
- [x] Get price at the end of 2018 for all stocks with a price for the end of 2015. 
- [x] Clean data
    - [x] 2018-close-price.tsv
    - [x] price-split-adjusted.csv
    - [x] fundamentals.csv
    - [x] securities.csv
- [x] Calculate growth for every stock that has a price at the end of 2015 and the end of 2018.
- [x] Find the growth percentage cut off for the 80 percentile.
- [x] Summarize the stock price adjusted data set into growth per year for 2013 - 2015
- [x] Create a model that has all 3 years of fundamental data, growth data, and the categorization in one row for each stock.  
## Find a Good Machine Learning Model
- [x] Break into test data and training data.
- [x] Standardized values.
    - [x] Save scalar model to file.
    - [x] Use the scalar model to standardize values for the test data.
- [x] Create base case (Naive Predictor).
- [ ] Train models.
    - [x] Without PCA.
        - [x] SVC.
        - [x] K Nearest Neighbors.
        - [x] Decision Tree/ Random Forest.
    - [ ] With PCA.
        - [x] SVC.
        - [ ] K Nearest Neighbors.
        - [ ] Decision Tree/ Random Forest.
- [ ] Compare Trained Models.

## Notes
- Probably should make some graphs showing Average training time, average time to answer (not sure the technical term for this), or compare performance of the different models.
    - Be sure to call out hardware on any graphs that deal with training, or guessing time.
- Reference this [scikit-learn link](https://scikit-learn.org/stable/tutorial/machine_learning_map/index.html) for models to try.
- Make sure to try random forest decision trees and matrix training for tuning.
- If processing time is slow on the laptop consider using a large vm on the home server.
- Consider using PCA since there are 233 features for the 389 rows.
- Reference this [scikit-learn link](https://scikit-learn.org/stable/model_persistence.html) for ways to export models.