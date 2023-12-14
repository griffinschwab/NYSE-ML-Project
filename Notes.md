# General Notes and Thoughts

### How to categorize the data
I know I want to look for performance past 2016. I think tow years should be good. I can just do it on a year schedule and take the closing price on at the end of 2016 and the price at the end of 2018 and see how much growth occurred in that time period. As much as I recognize the fact that this is not what I would do if I was finding stocks for myself it can get the job done. I want to look for out performers so I can find the cutoff for the 95 percentile and make that a value on a table. After I have the categories then I just need to clean and wrangle the data into a usable format. steps are broken down below.

1. Get price at the end of 2018 for all stocks with a price for the end of 2016.
2. Calculate growth for every stock that has a price at the end of 2016 and the end of 2018.
3. Find the growth percentage cut off for the 95 percentile.
4. Create a csv with that true or false data from step 3.
5. Clean fundamentals and stock price adjusted data sets.
    - Make sure to remove stocks that don't have appear on the newly created csv
6. Summarize the stock price adjusted data set into growth per year for 2013 - 2016
7. Create a model that has all 4 years of fundamental data, growth data, and the categorization in one row for each stock.  
**Now you have your dataset**
8. Standardized values.
9. Break into test data and training data.
10. TBD... Have fun training models!
    - Probably should make some graphs showing Average training time, average time to answer (not sure the technical term for this), or compare performance of the different models.
        - Be sure to call out hardware on any graphs that deal with training, or guessing time.
    - Reference this [scikit-learn link](https://scikit-learn.org/stable/tutorial/machine_learning_map/index.html) for models to try.
    - Make sure to try random forest decision trees and matrix training for tuning.
    - If processing time is slow on the laptop consider using a large vm on the home server.
    - Create a private github repo for now and you can make it public later. This may be useful for organizing this todo list in issues.
    
    
