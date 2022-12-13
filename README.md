# [Grocerie Shopping pattern analysis](https://github.com/msbernal/groceries_analysis/blob/main/groceries_analysis.ipynb)

## Project Overview

In this project I worked with the Groceries Database to find patterns in the groceries consumption over the 2 years of data provided. The data provided is a relatively simple and clean dataset with which we can explore different time series techniques. 

## What you will find

1. EDA and data pre-processing using Python.
2. Stationarity and Tendencies analysis using Time Series Analysis with Python.
3. Market Basket Analysis using Apriori Algorithm in R.

## Main insights

The groceries database has 167 products sold throughout the 2 years of data registration. The 10 best-selling products represent around 36% of all units sold as seen in the chart below. 

![](https://github.com/msbernal/groceries_analysis/blob/main/assets/output_1.png)

Then I proceed to analyze the stationarity and tendencies of each product. Of the 10 best-selling products, only *Sausages* may have a significant trend or seasonality in their purchase. In particular, this product grew during 2015 with a marked trend, unlike the rest of the best-selling products.

![](https://github.com/msbernal/groceries_analysis/blob/main/assets/output_2.png)

Using the Apriori algorithm, I found 7 sets of products frequently bought together. From the association rules generated, we obtain some insights as:
- Buying *Sausages* usually induces the purchase of other products: packs or discounts could be made on this product.
- *Whole Milk* and *other vegetables* are also products that are purchased as a complement to others, as well as being in the top 10 best sellers.
- It is recommended to dedicate additional space on the shelves of these products, and reduce the space of those less purchased.
- The 7 most trusted rules/sets of products can be used to keep these products close to each other in the store.

A part of the association rules generated can be seen in the following graph: 

![](https://github.com/msbernal/groceries_analysis/blob/main/assets/output_3.png)

## Python Dependencies:
* [NumPy](http://www.numpy.org/)
* [Pandas](http://pandas.pydata.org/)
* [Matplotlib](http://matplotlib.org/)
* [Statsmodels](https://www.statsmodels.org/stable/index.html)

## R Packages:
* [Arules](https://cran.r-project.org/web/packages/arules/index.html)
* [ArulesViz](https://cran.r-project.org/web/packages/arulesViz/index.html)
