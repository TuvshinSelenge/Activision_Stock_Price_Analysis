![GitHub watchers](https://img.shields.io/github/watchers/TuvshinSelenge/Activision_Stock_Price_Analysis?style=plastic)

# Activision Stock Price Analysis 

+ Author: Tuvshin Selenge
+ ORCID: https://orcid.org/0009-0001-3293-2959
+ Year of Creation: 2023
+ Subject: Stock Price Analysis with Python

---
**Overview**

This project analyzed the relationship between game releases, user ratings, and Activision's stock price performance. Data was collected from the Steam Store and SteamSpy APIs, leveraging existing datasets compiled by other users. The collected data included details on games available on the Steam platform, such as genres and estimated number of owners. Historical price data for Activision was also obtained from a Kaggle user's open-source API. A rating formula provided by SteamDB was implemented to assign ratings to Activision games based on user votes. 
Python and relevant packages were used for analysis, focusing on the impact of highly-rated game releases on stock market performance.

**Key Topics**

 - Dataset Overview
 - Data Organisation
 - Code
 - Conculusion

---
**Dataset Overview**

Dataset attributes: steam.csv

+ Type: Comma-separated values
+ Columns:   appid, name, release_date, english, developer, publisher, platforms, required_age, categories, genres, steamspy_tags, achievements, positive_ratings, negative_ratings, average_playtime, median_playtime, owners and price.
+ Rows: 27.076

Dataset attributes: act_bliz.csv

+ Type: Comma-separated values
+ Columns: Date, Open, High, Low, Close, Volume and Currency
+ Rows: 3.192

---
**Data Organisation**

The original datasets used in this project were sourced from Kaggle. However, the creators of the original datasets did not provide DOIs for them. In order to ensure proper identification and accessibility, DOIs were created specifically for these datasets in the context of this project.

The project utilizes Digital Object Identifiers (DOIs) to uniquely identify and reference the datasets. The assigned DOIs for the datasets in this project are:

**steam**

+ [10.5281/zenodo.7904761](https://doi.org/10.5281/zenodo.7904761) 

**act_bliz**

+ [10.5281/zenodo.7904772](https://doi.org/10.5281/zenodo.7904772) 

These DOIs serve as persistent identifiers, allowing others to easily locate, cite, and access the datasets even though the original creators did not provide DOIs themselves.

By creating DOIs for the datasets sourced from Kaggle, this project ensures that the datasets are properly identified and discoverable. Users can confidently refer to the DOIs provided to access and utilize the datasets in their own analyses and research.

**Original sources** from Kaggle:

**Steam Games**: https://www.kaggle.com/datasets/nikdavis/steam-store-games?resource=download&select=steam.csv

**Activision Stock Price**: https://www.kaggle.com/datasets/psycon/game-companies-historical-stock-price-2022-04?select=act_bliz.csv

---
**Code**

The project utilizes Python programming language in a Jupyter Notebook environment. 
The essential packages employed are **pandas, numpy, matplotlib, math, yfinance, and datetime**.
Python is used for data manipulation and control processes, leveraging pandas and numpy for efficient handling of datasets. The matplotlib package is utilized for data visualization, providing various charting options for insightful graphical representations.

The math package plays a crucial role in calculating ratings, which are derived using a formula obtained from SteamDB, a reputable third-party provider for Steam data. The specific formula can be found in their blog entry at: https://steamdb.info/blog/steamdb-rating/.

Furthermore, to enrich the dataset and ensure a comprehensive analysis, additional stock price data for Activision is downloaded from the yfinance API provided by Yahoo. The data covers the period from the beginning of 2006 to the end of 2009. This data supplementation is necessary to complete any missing values in the existing dataset obtained from the "act_bliz.csv" file. 

The downloaded data will be merged with the existing dataset, filling in any gaps and providing a more comprehensive timeline for analysis. This integration of historical stock price data obtained from the yfinance API enhances the accuracy and completeness of the analysis, ensuring that the impact of game releases on Activision's stock price is examined within a comprehensive timeframe.

*Side Note: Each significant part of the code is thoroughly explained with comments, providing clear explanations and guidance throughout the implementation. These comments serve to enhance code readability, comprehension, and facilitate understanding of the various processes and calculations involved.*

---
**Conclusion**

This research aims to provide valuable insights into the dynamics of Activision's stock price. By examining the interplay between game releases, user ratings, and stock market performance, it sheds light on the factors influencing Activision's stock price. Through the analysis and interpretation of relevant charts, this project contributes to a deeper understanding of the intricate relationship between highly-rated game releases and stock performance. 

The findings and observations derived from this study serve as valuable resources for comprehending gaming industry trends and the financial performance of companies like Activision. With this comprehensive analysis, we conclude our exploration into the captivating connection between gaming and stock markets.
