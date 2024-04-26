# New York Stock Exchange Machine Learning Project
This is a machine learning project using New York Stock Exchange data.

## Purpose
The goal of this project is to create a machine learning model that will predict which publicly traded companies will outperform most of the market. The target F-score with a beta of 0.5 is 80 percent. 

## Notebooks
- [clean-and-wrangle-data](./clean-and-wrangle-data.ipynb)
    - This notebook is for cleaning and wrangling the below data files into one output CSV.
    - **Outputs**
        - A final data model in a csv file. This final file will consist of one row per stock. File location will be `./outputs/data/finalmodel.csv`.
- [train-and-test-ml-models](./train-and-test-ml-models.ipynb)
    - This notebook is where the training of the ML models will take place.
    - Three algorithms will be used
        - Support Vector Classifier (SVC)
        - K nearest neighbors
        - Random forest decision trees
    - Each Model will be trained on time without and one time with Principal Component Analysis (PCA) dimensional reduction.
    - **Outputs**
        - A joblib file for each SciKit-Learn model that gets trained. This is so that you can run test on the models with out having to train them again. These files are save in `./outputs/models/`.
        - A CSV file with the measured performance of each ML model. This file is saved as `./outputs/data/model-performance.csv`. 

## The Data
- From [Kaggle.com](https://www.kaggle.com/datasets/dgawlik/nyse)
- [2018-close-price](./data/raw/2018-close-price.tsv): Stock prices for the last day the market was open in 2018. This was gathered using Google Finance.
- [fundamentals](./data/raw/fundamentals.csv): Stock fundamentals data for each stock. each stock has about four years worth of data but not all for the same years.
- [prices-split-adjusted](./data/raw/prices-split-adjusted.csv): Consist of the closing price for each stock for each day from 2010 through 2016.
- [securities](./data/raw/securities.csv): Some additional meta data for each stock.

### Disclaimer
> This is for demonstration purposes only. Please do not use this to actually guide any investment decisions. This is not to be used to make any real world investment decisions.