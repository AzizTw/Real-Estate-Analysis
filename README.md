# Introduction

This dataset, sourced from [aqar.fm](https://sa.aqar.fm/), provides a comprehensive collection of real estate listings in Saudi Arabia. It includes properties available for sale or rent and covers a wide range of listing attributes and pricing information. The dataset represents all publicly accessible listings up until the date of collection (2023/05/03).

The dataset was downloaded from [Kaggle](https://www.kaggle.com/datasets/mohdph/saudi-arabia-real-estate-dataset) - `database.db (969.8 MB)`

#### Why Did I Choose This Dataset?

1. Size: The dataset offers a substantial amount of data (~500k records), providing a rich and comprehensive resource for analysis and modeling.
2. Multiple Attributes and Layers: The dataset includes numerous attributes and layers, allowing forin-depth exploration and the potential to uncover valuable insights.
3. Data Quality: The dataset is not clean, which presents an opportunity to apply data cleaning techniques and enhance the data quality for accurate analysis.

By considering these factors, this dataset was selected as it presents an excellent opportunity for comprehensive analysis, insightful discoveries, and the development of robust models.

# Objective

The objective is to draw some insights from the data and try to build a model that can predict the price of a property based on its features.

# Conclusion

With this dataset taken from Kaggle which was scrapped from aqar.com, our objective was to predict the price of a property given some features. We started by exploring the data and visualizing it. Then we did some feature engineering and preprocessing. And finally we built a model and evaluated it.

Some insights we got from this analysis:

1. Riyadh, Jeddah and Dammam have the most listings. Which is expected.
2. Al Mubarraz, Al Wadiah and Anak have the least listings.
3. Al Diriyah, Al Riyadh and [Tarout](https://ar.wikipedia.org/wiki/%D8%AA%D8%A7%D8%B1%D9%88%D8%AA_(%D8%AC%D8%B2%D9%8A%D8%B1%D8%A9)) are the most expensive cities on average.
4. The most common categories are Villa for sell, Land for sell, Apartment for sell and Apartment for rent.
5. Properties for sell are significantly more expensive than properties for rent.
6. The average price of the category was correlated with the price. Followed by the average price of the district.
7. The average price of the category was the most important feature in predicting the price. Followed by the average price of the district and the city.

Finally, we trained our XGBoost model and got a score of 0.8916 on testing data. Which means that our model can capture/explain **89.16%** of the variance in the testing data.

# Library Versions

- **NumPy**: 1.22.3

- **Pandas**: 1.4.2

- **Matplotlib**: 3.5.1

- **Seaborn**: 0.11.2

- **SQLite3**: 2.6.0

- **Scikit-Learn**: 1.0.2

- **XGBoost**: 1.7.4

- **Arabic Reshaper**: 3.0.0

- **Python-Bidi**: 0.4.2
