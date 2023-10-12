# TUMO LABs
# Model Building, Evaluation and Validation
## Project:  Future-Sales-Prediction

### Install

This project requires **Python** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

You will also need to have software installed to run and execute a [Jupyter Notebook](http://jupyter.org/install.html).

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](https://www.anaconda.com/download/) distribution of Python, which already has the above packages and more included. 

### Code

Template code is provided in the `FutureSalesPrediction.ipynb` notebook file. You will also be required to use the included `FutureSalesPrediction.ipynb` Jupyter Notebook  file and the `advertising.csv` dataset file to complete your work.

### Run

In a terminal or command window, navigate to the top-level project directory `boston_housing/` (that contains this README) and run one of the following commands:
```bash
ipython notebook boston_housing.ipynb
```  
or
```bash
jupyter notebook boston_housing.ipynb
```
or open with Juoyter Lab
```bash
jupyter lab
```

This will open the Jupyter Notebook software and project file in your browser.

### Data
The Advertising dataset consists of (200, 4) row & columns.We are going to  use the advertising dataset given in ISLR and analyse the relationship between 'TV,Radio & Newspaper advertising' and 'Sales' using a simple linear regression model. Each row in the dataset represents a different advertising campaign, and the columns represent various features related to those campaigns.



**Features**
1.  `TV`:  this column represents the amount of money spent on TV advertising (in thousands of dollars) for each campaign. It measures the advertising budget allocated to television commercials.
2. `Radio`: this column represents the amount of money spent on radio advertising (in thousands of dollars) for each campaign. It measures the advertising budget allocated to radio commercials.
3. `Newspaper`:  this column represents the amount of money spent on newspaper advertising (in thousands of dollars) for each campaign. It measures the advertising budget allocated to newspaper ads.

**Target Variable**
4. `Sales`:this column represents the sales generated (in thousands of units) as a result of each advertising campaign. It measures the effectiveness of the advertising in driving product sales.

This type of analysis helps businesses make informed decisions about how to allocate their advertising budgets for maximum sales impact.
The detailed comments about the output examples  on each step you can find in the `FutureSalesPrediction.ipynb` notebook file.

# The results of  model: accuracy and prediction for the given project
## Summary
1.  `R-squared and adjusted R-squared :` 0.903 and 0.901 - with \"90%\" the model predicts accurately.
2. `F-stats and Prob(F-stats) (overall model fit)` - 605.4 and 8.13e-997 (approx. 0.0) - Model is significant and the explained \"90%\" accuracy is not random.
3. `p-values` - p-values for all coefficients except Newspaper are less than 0.05 significance level, which means that all predictors are statistically significant.
4. The relationship between the independent variables and the dependent variable is `linear`. This assumption is supported by a high R-squared value indicating that the model fits the data well. 
5. `Homoscedasticity.` The variance of the residuals is constant across all values of the independent variables. A Durbin-Watson statistic is close to 2, it suggests that the assumption of independence of residuals is likely met, and there is no significant autocorrelation. 
6. `Normality.` the residuals are normally distributed. This assumption confirms the Jarque-Bera statistic (the Jarque-Bera test statistic is always positive, and if it is not close to zero, it indicates that the sample data does not have a normal distribution.) 
7. `Independence.` the residues are independent of each other. This assumption is supported by the absence of autocorrelation in the residuals.

`We applied the model we built to new data and got predictions`

|        | Actual    | Predicted |
| ------ | --------- |  ---------|
| 123    | 15.2      | 15.072942 |
| 37     | 14.7      | 14.134829 |
| 4      | 17.9      | 15.547703 |
| 138    | 9.6       | 9.802572 |
| 17     | 24.4      | 24.160206 |
| 145    | 10.3      | 12.355845 |
| 177    | 16.7      | 14.632658 |
| 90     | 14.0      | 12.367404 |
| 83     | 13.6      | 13.245804 |
| 110    | 18.4      | 17.676377 |
| -----  |  -------- | --------- |

To provide a summary,let calculate some common metrics used to evaluate the performance of predictive models. The most commonly used metrics for regression tasks are Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE). Here are the calculations:
Mean Absolute Error (MAE):
MAE measures the average absolute difference between the actual and predicted values.
Formula: MAE = (1/n) * Σ|actual - predicted|
`Calculated MAE for your data: 2.398`

Mean Squared Error (MSE):
MSE measures the average squared difference between the actual and predicted values. It gives more weight to large errors.
Formula: MSE = (1/n) * Σ(actual - predicted)^2
`Calculated MSE for your data: 8.676`

Root Mean Squared Error (RMSE):
RMSE is the square root of MSE. It's a commonly used metric because it's in the same units as the target variable, making it easier to interpret.
Formula: RMSE = √MSE
`Calculated RMSE for your data: 2.946`

These metrics provide a summary of how well  model's predictions match the actual values. Lower values of MAE, MSE, and RMSE indicate better model performance. In this case, a lower RMSE suggests that the model's predictions are generally close to the actual values.



### Have questions, contact me.
[![LinkedIn](https://img.shields.io/static/v1.svg?label=connect&message=@monica-avagyan&color=success&logo=linkedin&style=flat&logoColor=white&colorA=blue)](https://www.linkedin.com/in/monica-avagyan/)


[![GitHub](https://img.shields.io/static/v1.svg?label=connect&message=@monicaavagyan&color=success&logo=github&style=flat&logoColor=white&colorA=blue)](https://github.com/monicaavagyan)

:email: Feel free to contact me @ [avagyanmonika3@gmail.com](https://mail.google.com/mail/)
