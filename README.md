# Applied_Data_Science_Clustering-Filtering
## IMDB Movies Dataset Analysis Report
This report provides a comprehensive analysis of the IMDB Top 1000 Movies dataset. It focuses on extracting insights, descriptive statistics, and visualization of important metrics like IMDb ratings, gross earnings, genres, and clustering patterns.
## 1. Dataset Overview
The dataset contains the following attributes:
<br>Series_Title: Title of the movie.
<br>Released_Year: Year the movie was released.
<br>Certificate: Age rating of the movie.
<br>Runtime: Duration of the movie in minutes.
<br>Genre: Genres associated with the movie.
<br>IMDB_Rating: IMDb rating (out of 10).
<br>Meta_score: MetaCritic score (out of 100).
<br>Director: Director of the movie.
<br>Stars: The top 4 actors/actresses of the movie.
<br>No_of_Votes: Number of votes received by the movie on IMDb.
<br>Gross: Box office gross earnings in USD.
## 2. Key Insights from the Dataset
### 2.1 Top 5 Movies by IMDb Rating
<br>The following movies have the highest IMDb ratings:
<br>The Shawshank Redemption - IMDb Rating: 9.3
<br>The Godfather - IMDb Rating: 9.2
<br>The Dark Knight - IMDb Rating: 9.0
<br>The Godfather: Part II - IMDb Rating: 9.0
<br>12 Angry Men - IMDb Rating: 9.0
### 2.2 Genre Distribution
The dataset reveals the popularity of various genres in the top 1000 movies. The top genres and their frequency are as follows:
<br>Drama: 724 movies
<br>Comedy: 233 movies
<br>Crime: 209 movies
<br>Adventure: 196 movies
<br>Action: 189 movies
### Visualization:
A bar chart was plotted to display the distribution of genres, showing that Drama is the most popular genre, followed by Comedy and Crime.
### 2.3 Descriptive Statistics
Key statistics for numerical columns (IMDb Rating, Runtime, and Gross Earnings):
<br>Average IMDb Rating: 7.93
<br>Average Runtime: 122.89 minutes
<br>Average Gross Earnings: $68,034,750.87
<br>Correlation Analysis:
<br>A heatmap was generated to explore the relationships between key numerical features like IMDb Rating, Runtime, Gross Earnings, and Meta Score.
<br>IMDb Rating is weakly correlated with Gross Earnings (positive correlation).
<br>Meta Score and IMDb Rating show a moderate positive correlation.
### 2.4 IMDb Rating vs. Gross Earnings
A scatter plot was created to explore the relationship between IMDb Rating and Gross Earnings.
<br>Trend: A positive trend is observed where movies with higher IMDb ratings tend to earn more, although the relationship is not strong.
<br>Regression Line: A linear regression line was added to quantify the trend, with the R² value indicating the strength of the relationship.
## 3. Clustering Analysis
### 3.1 KMeans Clustering
Clustering was performed on two features: IMDb Rating and Gross Earnings. The dataset was standardized to account for the large scale difference between these features.
<br>Number of Clusters: 2 (determined using the silhouette score).
<br>Cluster Centers: The cluster centers were computed and then scaled back to the original values for interpretation:
<br>Cluster 1: Low IMDb Rating and Low Gross Earnings
<br>Cluster 2: High IMDb Rating and High Gross Earnings
### Visualization:
A silhouette plot was created to validate the clustering quality. The average silhouette score showed that the clustering was moderately effective.
<br>A scatter plot with color-coded clusters was also generated, showing how movies were grouped based on the two features.
## 4. Visualizations and Insights
### 4.1 Genre Distribution
<br>Graph Type: Bar Chart
<br>Insight: Drama is the dominant genre, followed by Comedy and Crime.
![image](https://github.com/user-attachments/assets/364d6a3e-a47d-40a4-a428-5a88513fcf6e)
### 4.2 Correlation Heatmap
<br>Graph Type: Heatmap
<br>Insight: IMDb Rating correlates moderately with Meta Score but weakly with Gross Earnings.
![image](https://github.com/user-attachments/assets/cc7ddd76-29f3-436b-bac2-1e3780026d8d)
### 4.3 IMDb Rating vs. Gross Earnings
<br>Graph Type: Scatter Plot
<br>Insight: Movies with higher IMDb ratings generally earn more gross revenue, though exceptions exist.
![image](https://github.com/user-attachments/assets/de54c043-77da-4633-8da9-a01d6c5c2f89)
### 4.4 Clustering
<br>Graph Type: Silhouette Plot and Scatter Plot
<br>Insight: Movies were grouped into three clusters. The clusters represent different groupings of IMDb Ratings and Gross Earnings.
![image](https://github.com/user-attachments/assets/ee1d5c59-c8ea-4394-babd-ccbddf32e442)
### 4.5 Line Fitting
**Linear Model:** The linear model, while simple, does not fully explain the relationship between IMDb Rating and Gross Earnings, as evidenced by the low R² value. However, it provides a basic understanding of the positive trend.
**Quadratic Model:** The quadratic regression captures the curvature of the data better, suggesting that the relationship between IMDb Rating and Gross Earnings may not be perfectly linear. As IMDb Ratings rise, Gross Earnings initially increase, but the effect seems to plateau or diminish as ratings become very high.
**Statistical Significance:** The high statistical significance (low p-value) suggests that the relationship between IMDb Rating and Gross Earnings is real, though the strength of this relationship is modest.
![image](https://github.com/user-attachments/assets/dc5c7815-9a07-4904-891c-1582b20315ef)
![image](https://github.com/user-attachments/assets/4df2b440-9117-446a-900a-9577c12b1e0f)
## 5. Recommendations
**For Movie Studios:** Focus on producing high-quality movies with higher IMDb ratings to increase revenue potential.
<br>**For Analysts:** Further investigate how other factors (e.g., genre, director) influence Gross Earnings.
<br>**For Data Scientists:** Use additional clustering techniques (e.g., DBSCAN or hierarchical clustering) to validate the current results.
## 6. Conclusion
The analysis provides valuable insights into the top 1000 movies, revealing trends in ratings, earnings, and genre preferences. The visualizations and clustering add depth to the understanding of movie performance metrics. This information can be used by studios, marketers, and analysts to make informed decisions.
