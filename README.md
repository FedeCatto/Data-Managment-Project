The project follows the key stages of a structured data management process.
Data acquisition involved collecting both structured and unstructured information through web
scraping (using BeautifulSoup and Selenium) and APIs. We extracted detailed statistics from
sources such as Transfermarkt and FBref.com, and complemented them with contractual details
from API.football-data.org. These heterogeneous data sources were integrated and enriched
into a unified dataset using unique player identifiers and outer joins, combining performance
metrics, economic values, and contract information.
Data preparation included standardizing market values, processing contractual data, imputing
missing values, recoding variables and normalizing player positions.
A detailed data quality assessment was conducted to enhance completeness, consistency and
accuracy.
For persistent storage, a relational SQL database was employed, chosen for its ability to maintain data integrity, structured schema and compatibility with machine learning workflows.
Exploratory Data Analysis (EDA) was performed to identify trends, relationships and anomalies for predictive modeling. The core of the project was the development of a database for a
CatBoostRegressor model to estimate players’ market value based on their performance statistics. The model was trained and validated using Leave-One-Out Cross-Validation (LOOCV),
achieving a mean absolute error (MAE) of approximately € 4.2 million on held-out players.
Results revealed that the model tends to underestimate high-profile players while overestimating
lesser-known ones, indicating that intangible factors such as media attention and commercial
appeal—absent from the included features—affect extreme market valuations. Feature importance analysis highlighted age, team affiliation, remaining contract length and team success
metrics as the main drivers of predicted market value.
Overall, the project delivers a data-driven tool that can assist football clubs in identifying
pricing inefficiencies and supporting more informed transfer strategies, providing an objective
perspective on player valuation in professional football.
