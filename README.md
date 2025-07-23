# Football Player Market Value Estimation - Data Management Project

## Overview
This project follows a structured data management process to create a comprehensive dataset and predictive model estimating professional football players' market value based on performance and contract data.

## Data Acquisition
- Collected structured and unstructured data using **web scraping** (BeautifulSoup, Selenium) and **APIs**.
- Extracted detailed player statistics from sources like Transfermarkt and FBref.com.
- Integrated contractual and economic details via API.football-data.org.
- Unified diverse data sources using unique player IDs and outer joins.

## Data Preparation
- Standardized market values and processed contractual data.
- Imputed missing values and recoded variables.
- Normalized player positions for consistency.
- Performed thorough data quality assessments to improve completeness and accuracy.

## Storage and Tools
- Used a **relational SQL database** for persistent storage, ensuring data integrity and compatibility with machine learning workflows.

## Exploratory Data Analysis (EDA)
- Identified key trends, relationships, and anomalies in the dataset to inform model development.

## Predictive Modeling
- Developed a **CatBoostRegressor** model to predict player market value based on performance metrics.
- Trained and validated the model using **Leave-One-Out Cross-Validation (LOOCV)**.
- Achieved a mean absolute error (MAE) of approximately €4.2 million on held-out players.

## Results and Insights
- The model tends to underestimate high-profile players and overestimate lesser-known players.
- This suggests missing intangible factors like media attention and commercial appeal affect valuations.
- Feature importance analysis highlighted:
  - Age
  - Team affiliation
  - Remaining contract length
  - Team success metrics  
  as the main drivers of predicted market value.

## Conclusion
This project provides a data-driven tool to assist football clubs in identifying pricing inefficiencies and supporting informed transfer strategies by offering an objective perspective on player valuation.




