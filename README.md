                                                                             STOCK MARKET PREDICTION


APPROACH and METHODOLOGIES:

1.Data Import and Exploration:

   - The analysis begins with importing the dataset 'infolimpioavanzadoTarget.csv' using Pandas.
   - The shape of the dataset is checked to understand its dimensions.
   - The first few rows of the dataset are examined to get a glimpse of the data structure.
   - Information about the dataset, including data types and missing values, is obtained using the 'info()' function.
   - The number of missing values in each column is calculated using 'isna().sum()'.

2.Data Preprocessing:

   - Necessary columns for analysis are selected based on relevance to stock price prediction.
   - Duplicate rows are removed to ensure data integrity.
   - The 'date' column is converted to datetime format for temporal analysis.
   - Missing values are handled by either dropping or imputing them with mean values.
   - Additional features such as moving averages, technical indicators (RSI, MACD, Stochastic), and derived features are calculated to enrich the dataset.

3.Exploratory Data Analysis (EDA):
   - Various EDA techniques are employed to understand the distribution and relationships within the data.
   - Line plots, bar plots, histograms, and scatter plots are utilized to visualize stock prices, trading volumes, and their relationships with other variables.
   - Correlation matrices and heatmaps are generated to identify correlations between features and to detect multicollinearity.

4.Feature Selection:
   - Feature selection techniques like SelectKBest and Recursive Feature Elimination (RFE) are applied to identify the most relevant features for modeling.
   - Features are selected based on their importance scores, correlation coefficients, and coefficients from linear regression models.

5.Model Training and Evaluation:
   - Three predictive models, namely Linear Regression, Random Forest Regressor, and Gradient Boosting Regressor, are trained using the selected features.
   - The models are evaluated using common regression evaluation metrics like Mean Squared Error (MSE) and R-squared (R²).
   - A trained Linear Regression model is saved to a file ('linear_regression_model.pkl') for future use.

INSIGHTS:

 1 .Average trade volume was higher in 'Monday' and lower in 'Thursday' of the week.
 2 .Total trade volume was extremely high in the month of 'March' and lower in the month of 'January'.
 3 .Average price rise is higher at 'Monday' and lower at 'Tuesday'.
 4 .Average price rise is higher in the month of 'October' and lower in the month of 'April'.
 5 .Stock 'low price' is directly proportional to stock 'high price'.
 6 .Average close price was high in the month of 'January' and lower in the month of 'September'.
 7 .Close price was greater than 100 rarely.
 8 .Close price frequency was maximum in the area of '0-25'.
 9 .Daily price change(%) frequency range was between '0-17'.
 10.'open','high','low','close','adjclose','low-5','high-5', These column are always depend on each other.






                                                                            
