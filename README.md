# New York Stock Exchange Machine Learning Project
This is a machine learning project using New York Stock Exchange data.

## Steps To Take
1. [x] Get price at the end of 2018 for all stocks with a price for the end of 2016. 
2. [ ] Calculate growth for every stock that has a price at the end of 2016 and the end of 2018.
3. [ ] Find the growth percentage cut off for the 95 percentile.
4. [ ] Create a csv with that true or false data from step 3.
5. [ ] Clean fundamentals and stock price adjusted data sets.
    - Make sure to remove stocks that don't have appear on the newly created csv
6. [ ] Summarize the stock price adjusted data set into growth per year for 2013 - 2016
7. [ ] Create a model that has all 4 years of fundamental data, growth data, and the categorization in one row for each stock.  
**Now you have your dataset**
8. [ ] Standardized values.
9. [ ] Break into test data and training data.
10. [ ] TBD... Have fun training models!
    - Probably should make some graphs showing Average training time, average time to answer (not sure the technical term for this), or compare performance of the different models.
        - Be sure to call out hardware on any graphs that deal with training, or guessing time.
    - Reference this [scikit-learn link](https://scikit-learn.org/stable/tutorial/machine_learning_map/index.html) for models to try.
    - Make sure to try random forest decision trees and matrix training for tuning.
    - If processing time is slow on the laptop consider using a large vm on the home server.
    - Create a private github repo for now and you can make it public later. This may be useful for organizing this todo list in issues.