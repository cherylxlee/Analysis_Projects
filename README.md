# Data Analysis Projects

<img src="https://img.shields.io/badge/-Python-blue" /> <img src="https://img.shields.io/badge/-Jupyter-orange" />

## Sources
Inspiration and Tutorial from [Alex the Analyst](https://github.com/AlexTheAnalyst/PortfolioProjects)

## Movie Industry Analysis 🎬
Analysis of movie industry revenue over recent decades.

## Sources
[Kaggle Dataset](https://www.kaggle.com/datasets/danielgrijalvas/movies)

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
<img src="demo/m3.png" width="400" height="350" />
* There seems to be a positive trend indicating that films with higher budgets often have higher gross earnings.
* A cluster of data points can be seen toward the lower left, which suggests that a large number of films have both low budgets and low earnings.
* There are a few films with high gross earnings that do not necessarily have a high budget, indicating that some films can be highly profitable without massive investments.
* Several outliers can be observed where films have a high budget but don’t correspondingly have high gross earnings, indicating a potential lack of profitability for these cases.

### Correlation Matrix for Movies
<img src="demo/m4.png" width="400" height="350" />
Analyzing the correlation matrix:
* The correlation between budget and gross earnings is 0.74, reinforcing the idea seen in the scatter plot that a higher budget is moderately strongly correlated with higher gross earnings.
* There is a significant positive correlation (0.63) between the number of votes a movie receives (which can be an indicator of popularity or viewership) and its gross earnings.
* The score (perhaps a measure of critical acclaim or audience rating) has a positive correlation (0.19) with gross earnings but is not as strong as the budget or votes, indicating that while quality or reception is important, it may not be as strong a predictor of financial success as the other two factors.
* There is a notable correlation between runtime and gross earnings (0.25), suggesting that longer movies may have a tendency to earn more, perhaps because they are often major productions or have more content for viewers.
* The variable Year (which seems to be at the bottom of the matrix), presumably indicating the year of release, has no color coding associated with it, suggesting either it is not properly correlated with the other variables, or there might be an error in how the data is presented in this matrix.

