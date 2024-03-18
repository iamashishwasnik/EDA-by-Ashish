### Author-ASHISH WASNIK
# Title: Black Friday Sales Analysis and Prediction
![0_-e6G_N1MSr4CbEkK (1)](https://github.com/iamashishwasnik/EDA-of-Black-friday-sales-prediction-by-Ashish/assets/147370129/36a308de-984f-4896-965f-1e52e158aeda)

### Introduction:
Black Friday, a renowned shopping event following Thanksgiving Day, marks the commencement of the holiday shopping season with remarkable discounts and promotions. My project delves into the analysis of Black Friday sales data to unravel consumer trends and optimize pricing strategies for retailers. By harnessing machine learning algorithms, I endeavor to predict purchase amounts based on historical sales data, empowering businesses to make informed decisions and enhance profitability during this crucial sales event.

### Dataset Description:
The dataset, sourced from a Black Friday sales database, comprises various attributes such as User ID, Product ID, Gender, Age, Occupation, City Category, Stay in Current City Years, Marital Status, and Product Categories. With over 550,000 entries and 12 columns, including both categorical and numerical features, the dataset provides a comprehensive view of consumer behavior and purchasing patterns during Black Friday sales.

### Data Preprocessing:

* Handling missing values involves imputing missing values in Product_Category_2 and Product_Category_3 columns and dropping columns with significant missing data.:

* Categorical columns such as Gender, Age, City_Category, and Stay_In_Current_City_Years are encoded using LabelEncoder to convert them into numerical format for modeling purposes.

* Skewness treatment is applied to numerical columns like Product_Category_1 using PowerTransformer to normalize the distribution and improve model performance.

* Outlier treatment using the Interquartile Range (IQR) method ensures data integrity and enhances the reliability of predictive models by mitigating the impact of extreme values.

### Model Building and Evaluation:

* Linear Regression Model: The linear regression model achieved an R-squared score of approximately 0.18, indicating that around 18% of the variance in the purchase amounts can be explained by the features included in the model. However, the mean squared error (MSE) and mean absolute error (MAE) are relatively high, suggesting that the model's predictions deviate significantly from the actual purchase amounts.

* Decision Tree Regressor Model: The decision tree regressor model performed better than linear regression, achieving an R-squared score of about 0.75. This indicates that approximately 75% of the variance in purchase amounts is explained by the features in the model. The MSE and MAE are lower compared to linear regression, indicating better performance in predicting purchase amounts.

* Random Forest Regressor Model: The random forest regressor model further improved the predictive performance with an R-squared score of approximately 0.61. This suggests that the model accounts for approximately 61% of the variance in purchase amounts. The MSE and MAE are also lower compared to the linear regression model, indicating better predictive accuracy.

* K-Nearest Neighbors Regressor Model: The K-nearest neighbors regressor model achieved an R-squared score of around 0.66, indicating that approximately 66% of the variance in purchase amounts is explained by the features in the model. The MSE and MAE are lower compared to linear regression, suggesting improved predictive accuracy.

Overall, the decision tree, random forest, and K-nearest neighbors regressor models outperform the linear regression model in predicting purchase amounts during Black Friday sales. Among these, the K-nearest neighbors regressor model demonstrates the highest predictive performance based on the R-squared score and error metrics. Therefore, it may be the most suitable model for predicting purchase amounts in similar sales events.









