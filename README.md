# Outline

This repository is the final project for the course: CIS 545 Big Data Analytics at the University of Pennsylvania in 2021 Fall

# Group Member

* Meng-Chuan Chang
* Wei-Kai Chang
* Ru-Xuan Ji

# Dataset file

The following two main files do not upload to Github since those files are too large, so you need to go to Kaggle and download the dataset on your own. (All links are available in our notebook file)

* `/dataset/financial/stock_prices_latest.csv`
* `/dataset/text/tweet/Tweet.csv`

# Abstract

Stock prediction is always a hot topic as everyone wants to win money from the stock market and stock forecasting models have important value in the field of quantitative finance.

Nowadays, people begin to dine useful information for stock trading or prediction from all kinds of big data with big data analytics tools, machine learning methods or even deep learning. In our project, we build models for stock movement and stock price prediction with features including financial indicators and sentimental analysis from social networks.

First, we implement NLP models for text analysis on Tweets and headlines related to the companies listed in the datasets. With sentimental analysis, we analyze the correlations between news and market trends.

Second, some basic analysis is applied to the financial data. In this part, we analyze development of different sectors, correlation between different sectors and correlation between different financial indicators, which helps to select features for machine learning.

Finally, three types of machine learning models are built for stock trend prediction, including Random Forest, SVM and Logistic Regression.

# Conclusion

### Text Analysis

* Daily stock price movement are irrelevant to news headline
* Daily stock price movement are irrelevant to tweet comments (for top tech companies)
* Tweet can show what public thinks of a specific company and we can use big data analytics to capture the trend
* The number of News related to companies are far less than tweet since news are selected and often has their own preference (e.g. politics). Therefore, there might be some bias with the word frequencies and compound scores

### Fianancial data Analysis

* The data set we use exist large features and data amount trade off. To get more features, we need to sacrifice a lot of data.
* We can see in the analysis that the feature do not exist strong correlation between each other whcih is suitable for machine learning.

### Machine Learning

* The overall performance for differnet models is better than gaussing but not enough for practical usage.
* Hard to even overfit to the data, and this might indicate that the features are not useful for prediction.

| | Support Vector Machine | Random Forest | Logistic Regression |
|-|:-:|:-:|:-:|
|Without Text Data| 0.5923 | 0.6225 | 0.5647 |
|With Text Data| 0.5947 | 0.6264 | 0.5643 |

# Notebook File

For more detail such as the intermediate results or algorithm, you can see our code here: [Python/CIS545_Final_Project_Python.ipynb](Python/CIS545_Final_Project_Python.ipynb)

# Hyperlink

You can also visit my website to see the detail of our final project

* https://mcchanglife.com/project-upenn-cis-545/