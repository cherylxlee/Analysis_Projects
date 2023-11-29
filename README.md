# Data Analysis Projects

![Python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
![Pandas](https://img.shields.io/badge/-Pandas-blue?style=flat&logo=pandas)
![NumPy](https://img.shields.io/badge/-NumPy-lightgrey?style=flat&logo=numpy)
![SciPy](https://img.shields.io/badge/-SciPy-blue?style=flat)
![Matplotlib](https://img.shields.io/badge/-Matplotlib-black?style=flat&logo=matplotlib)
![Seaborn](https://img.shields.io/badge/-Seaborn-brightgreen?style=flat)

# Sources
Inspiration and Tutorial from [Alex the Analyst](https://github.com/AlexTheAnalyst/PortfolioProjects)

# Crypto API Automation Analysis 📈
Features fetching and analyzing cryptocurrency data from the CoinMarketCap API. Designed to be run periodically to collect the latest cryptocurrency listings and analyze their price trends over time.

### Key Features
- API Interaction: Uses `requests` library to interact with the CoinMarketCap API, handling potential connection errors gracefully.
- Data Normalization: Converts the received JSON data into a flattened `pandas` DataFrame for easier manipulation.
- Timestamping: Appends the current timestamp to the DataFrame entries to keep track of data retrieval time.
- Iteration for Data Collection: Implements a loop to continuously collect data.
- Data Visualization: Plots trends and insights, which are explored further below.

### Steps to Run the Project
1. Execute the script in a Jupyter notebook or other Python environment.
2. Install the required libraries.
3. After collecting the data, the script processes and visualizes it to identify trends.

### Dependencies
- `requests` for API calls
- `pandas` for data manipulation
- `scikit-learn` for linear regression
- `seaborn`, `matplotlib`, `plotly` for visualization

### Performance Over Time Intervals Analysis
![Interactive Analysis](demo/c1.png) 

This multi-line chart compares the performance of various cryptocurrencies over different time intervals, each line representing a different token. This chart is useful for visualizing which tokens are more volatile across different timescales.
#### Usage:
To analyze market trends, identify which cryptocurrencies are the most volatile, and observe the general market behavior over time. This can be particularly useful for investors and traders interested in analyzing performance over multiple time periods.

### Interactive Detailed Cryptocurrency Price Movement
![Interactive Analysis](demo/cv1.gif) 

This interactive line chart features a user-friendly interface that allows you to select different tokens to analyze their price movements within the detailed timeframe. Timeline can be adjusted for more or less granularity.
#### Usage:
For conducting an in-depth micro-analysis of selected cryptocurrency behavior, useful for developing or testing high-frequency trading algorithms. It's also valuable for researchers focused on the market microstructure of specific digital assets.

### Interactive Cryptocurrency Price Prediction
![Regression](demo/cv2.gif)  

This interactive chart offers a dynamic comparison between the actual and predicted prices of a user-selected cryptocurrency over a specified timeframe. Users can choose different tickers from a dropdown menu to view the corresponding data. The actual prices are plotted as black dots, while the predicted trend is shown in blue. The prediction model's trendline adjusts according to the selected cryptocurrency.
#### Usage:
Risk assessment. Comparing actual and predicted prices can be a critical tool for assessing the risk associated with different cryptocurrencies. A higher divergence between predicted and actual prices may indicate higher volatility and risk.

# Movie Industry Analysis 🎬
Analysis of a dataset containing movie industry data. Used Pandas, NumPy, Seaborn, and Matplotlib, to explore, visualize, and gain insight into movie trends. Dataset from [Kaggle](https://www.kaggle.com/datasets/danielgrijalvas/movies)

### Key Features
- Data Cleaning: Code ensures the data is in good shape, checking for missing data.
- Data Exploration: Code explores data types before any data manipulation.
- Outlier Detection: Includes functionality to detect outliers in key categories (gross revenue), important for accurate statistical analysis.

### Steps to Run the Project
1. Setup Environment: Ensure that Python is installed on your system and that you have installed the required packages (`pandas`, `numpy`, `seaborn`, and `matplotlib`).
2. Load Data: Place the `movies.csv` file in a known directory and adjust the path in the `pd.read_csv()` function.
3. Explore Data: Execute the script to load and explore the dataset using the commands provided.
4. Data Cleaning: The script will loop through each column to check for missing values and print out the percentage of missing data for each attribute.
5. Analyze Data Types: Use `print(df.dtypes)` to understand the types of data you are dealing with.
6. Visualize Data: Use `matplotlib` to create graphs, such as visualizing outliers in the gross revenue data.

### Enhancements
- Handling Outliers: Implement methods to handle outliers effectively, either by removing them or by using robust statistical methods.
- Advanced Visualizations: Create more sophisticated visualizations to uncover patterns and relationships in the data.
- Statistical Analysis: Perform statistical tests to validate hypotheses about the dataset.
- Predictive Modeling: Extend the script to include predictive analytics using machine learning libraries like `scikit-learn` to, for example, predict movie success based on given features.

### Scatter Plot of Budget vs. Gross Earnings
![Budget vs Gross Earnings Scatter Plot](demo/m1.png)  
Key observations from the scatter plot:
- A concentration of points towards the lower left corner indicates many movies have both lower budgets and gross earnings.
- An upward trend suggests a positive relationship between the budget and gross earnings.
- A wide confidence interval around the regression line suggests high variability beyond budget considerations.

### Correlation Matrix for Numeric Features
![Correlation Matrix](demo/m2.png)  
Insights from the correlation matrix:
- Budget and gross earnings share a strong positive correlation.
- Votes and gross earnings are moderately correlated, implying popular/talked-about movies tend to earn more.
- Score has a weaker positive correlation with gross earnings, suggesting that critical reviews do not necessarily predict earnings.

### Budget vs. Gross Earnings Scatter Plot
![Budget vs Gross Earnings Scatter Plot](demo/m3.png)  
Observations from the scatter plot:
- Some movies with high earnings don't necessarily have large budgets, implying high profitability is possible without significant investment.
- Outliers are present where films with high budgets don't have high gross earnings, which may point to flopping/underperformaing at the box office.

### Correlation Matrix for Movies
![Correlation Matrix for Movies](demo/m4.png)  
Key points from the correlation matrix:
- Runtime shows a notable correlation with earnings, hinting that longer movies might earn more, potentially due to being bigger productions.
- Year does not have a clear correlation, which could imply that audience's demand for movies on the big screen is consistently stable over time.
