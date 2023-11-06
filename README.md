# Data Analysis Projects

<img src="https://img.shields.io/badge/-Python-blue" /> <img src="https://img.shields.io/badge/-Jupyter-orange" />

## Sources
Inspiration and Tutorial from [Alex the Analyst](https://github.com/AlexTheAnalyst/PortfolioProjects)

## Movie Industry Analysis 🎬
Analysis of movie industry revenue over recent decades. Dataset from [Kaggle](https://www.kaggle.com/datasets/danielgrijalvas/movies)

### Scatter Plot of Budget vs. Gross Earnings
![Budget vs Gross Earnings Scatter Plot](demo/m1.png)  
Key observations from the scatter plot:
- A concentration of points towards the lower left corner indicates many movies have lower budgets and gross earnings.
- An upward trend suggests a positive relationship between the budget and gross earnings.
- A wide confidence interval around the regression line points to high variability beyond budget considerations.

### Correlation Matrix for Numeric Features
![Correlation Matrix](demo/m2.png)  
Insights from the correlation matrix:
- Budget and gross earnings share a strong positive correlation (0.69).
- Votes and gross earnings are moderately correlated (0.57), implying popular movies tend to earn more.
- Score has a weaker positive correlation with gross earnings (0.17), suggesting that higher ratings do not necessarily predict higher earnings.

### Budget vs. Gross Earnings Scatter Plot
![Budget vs Gross Earnings Scatter Plot](demo/m3.png)  
Observations from the scatter plot:
- Films with higher budgets often show a trend of higher gross earnings.
- A dense cluster of data points towards the bottom left signifies many films with low budgets and earnings.
- Some films with high earnings don't necessarily have large budgets, implying high profitability is possible without significant investment.
- Outliers are present where films with high budgets don't have high gross earnings, which may point to financial underperformance.

### Correlation Matrix for Movies
![Correlation Matrix for Movies](demo/m4.png)  
Key points from the correlation matrix:
- A 0.74 correlation between budget and gross earnings suggests a moderately strong positive relationship.
- The number of votes a movie receives has a significant positive correlation (0.63) with its gross earnings, indicating that more popular movies tend to be higher earners.
- The score has a positive correlation (0.19) with gross earnings, but it is not as predictive of success as budget or votes.
- Runtime shows a notable correlation (0.25) with earnings, hinting that longer movies might earn more, potentially due to being major productions.
- The 'Year' variable does not have a clear correlation, which could imply a data presentation issue or lack of significant correlation.
