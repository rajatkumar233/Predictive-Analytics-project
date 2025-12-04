# Predictive-Analytics-project
#About Dataset
This project uses the Online Shoppers Intention dataset to predict whether a visitor will make a purchase or not on an e-commerce website.

The goal is to understand which user behaviors lead to purchases and build a simple machine learning model that can classify sessions as purchase or no-purchase.

-> Project Objective

The main objective of this project is:

To study how users behave on an online shopping website

To identify which actions increase the chance of buying

To build a model that predicts Revenue = 1 (purchase) or 0 (no purchase)

To help improve user experience and reduce drop-offs

-> Dataset Details

The dataset contains 12,330 rows and 18 columns, including:
from OpenML website

-> Important Features

ProductRelated – number of product pages visited

ProductRelated_Duration – time spent on product pages

BounceRates – how often users leave after first page

ExitRates – how often users leave from a page

PageValues – importance of the page for conversion

Month – which month the user visited

VisitorType – New or Returning visitor

Weekend – True/False

-> Target Variable

Revenue

1 = user made a purchase

0 = user did not purchase

 -> Data Preprocessing

Steps performed in preprocessing:

Loaded the dataset using pandas

Checked for missing values (dataset is clean)

Converted Revenue from True/False → 1/0

One-hot encoded categorical columns:

Month

VisitorType

Weekend

Split dataset into Train (75%) and Test (25%)

-> Machine Learning Model Used

I used Random Forest Classifier because:

It is simple to use

Works well with mixed data (numeric + categorical)

Gives good accuracy on classification problems

The steps:

Fit the model on training data

Predict on test data

Evaluate using:

Accuracy

Classification Report

Confusion Matrix

-> Model Performance

The Random Forest model gave:

Accuracy: ~89–90%

Good prediction performance for both classes

Useful feature importance results

🔥 Most Important Features

PageValues

ProductRelated_Duration

ExitRates

BounceRates

Some months like November & December

These features strongly influence whether a user purchases.

💡 Key Insights (Easy Language)

Only around 15% of users actually purchase.

Users who spend more time on product pages are more likely to buy.

High bounce and exit rates reduce chances of purchase.

New visitors surprisingly convert more than returning visitors.

Months like October and November show higher conversion (due to festive sales).

🧩 Technologies Used

Python

Pandas, NumPy

Matplotlib

Scikit-Learn


Optimize website behavior

Identify high-intent users

Personalize recommendations
