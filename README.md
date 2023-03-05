# Yes-Bank-Stock-Closing-Price-Prediction

Yes Bank is a well-known bank in the Indian financial domain, headquartered in Mumbai, India and was founded by Rana Kapoor and Ashok Kapoor in 2004. Since 2018, it has been in the news because of the fraud case involving Rana Kapoor. Owing to this fact, it was interesting to see how that impacted the stock prices of the company and whether predictive models can do justice to such situations.

This dataset has monthly stock prices of the bank since its inception and includes closing, starting, hightest, and lowest stock prices of every month. The given dataset which contains 185 row labels with 5 variables including no missing and no duplicates values. The close pricing is considered as dependent variable and Open, high, low pricing are considered as independent variables.

The main objective is to predict the stock's closing price of the month.

First, data was loaded, we did the Exploratory Data Analysis where we tried to know about various variable and their relationship through the graphs like scatter plots to know about the linear relationship between dependent and independent variable, histogram with bell shaped curve to know about how the variable is distributed, box whisker plot, pair-wise plot, heatmap matrics etc. It was found that the given data was positively skewed. We tried different transformation. By using the log transformation, the given was normally distributed was shown in histogram. From the scatter plot, it was observed that Variance around the regression line is same at origin sided portion after that it is showing heteroscedasticity before the transformation. After the transformation, It means that the variance around the regression line is the same for all values of the predictor variables. We formed the assumption and obtained insights by visualizing of dependent variable (line graph) and hypothesis testing ( using parametric t-test) to give the strogest evidence how close pricing of nth day is corelated with (n+1) th day of opening price. We measured the amount of multicollinearity in regression analysis using Variance Inflation Factor (VIF). It was found that predictor variable showed multicollinearity but no variable was dropped as we had only 3 independent variable then we did data pre-processing. We did the feature engineering and data preprocessing.Finally, we implemented models like multiple liner regression, Ridge Regression, LASSO regression and Elastic Net Regression. We compared the implemented models by using performace merics which are MSE, RMSE, MAE, R squared score and adj. R squared score.
Finally, We came to conclusion:
1. Given dataset does not have missing values and duplicates values.

2. The closing price of stock is considered as dependent features whereas opening price, lowest price and highest price of stock are independent features.

3. Since 2018, yes bank had been in the news because of the fraud case involving the co-founder Rana Kapoor. This news directly impacted the stock price as a result the closing price fall down rapidly and come to zero at year 2020

4. Independent variables such as Low, Open, High are shown the linearity with dependent variable Close.

5. There is sufficient statistical evidence at the α = 0.05 level to conclude that there is a significant linear relationship between n th day closing price and (n+1)th of the opening price.

6. All the freatures are positively skewed distributed. Mean is greater than Median i.e Mean > Media.

7. After the log transformation, Distribution of features are similar to normal distribution. The mean and median values are nearly same. It diminishes the outlier's effect and heteroscedasticity.

8. In multiple linear regression, F cal > F tab (3, 181) so we reject the null hypothesis with 5 % level of significance. we conclude that the close price of stock is dependent of Highest, Lowest and Opening price of stock i.e ˆβ1 ≠ ˆβ2 ≠ ˆβ3 ≠ 0. It may be possible that estimate parameters are lossing preciseness as multicolineariy is considered.

9. The fit is good at LOS 5%. It means that all models fits a given testing set of data.

10. Several models are implemented on the given dataset in order to predict the closing price and found that Elastic net regression is the best performing model with adjusted R squared is 0.9931.

It was wonderful learning experience while working on this project. This project has developed thinking skills related to the topics. This project gave real insights. we enjoyed each and every moment. Thank You!
