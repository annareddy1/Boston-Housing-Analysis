# Boston-Housing-Analysis
The Boston dataset contains the housing values of 506 suburbs in the Boston area. The dataset contains 13 predictors and 1 mystery response variable that we will try to predict statistical analysis.

### Team members

Rithika Annareddy,
Cameron Erdman,
Colin Walsh,
Maggie Miller,
Zak Taylor

### Variables

The 13 predictors in this dataset are as follows:

- **CRIM**: Per capita crime rate by town.
- **ZN**: Proportion of residential land zoned for lots over 25,000 sq.ft.
- **INDUS**: Proportion of non-retail business acres per town.
- **CHAS**: Charles River dummy variable (= 1 if tract bounds river; 0 otherwise).
- **NOX**: Nitrogen oxides concentration (parts per 10 million).
- **RM**: Average number of rooms per dwelling.
- **AGE**: Proportion of owner-occupied units built prior to 1940.
- **DIS**: Weighted mean of distances to five Boston employment centers.
- **RAD**: Index of accessibility to radial highways.
- **TAX**: Full-value property-tax rate per $10,000.
- **PTRATIO**: Pupil-teacher ratio by town.
- **LSTAT**: Percentage of lower status of the population.
- **MEDV**: Median value of owner-occupied homes in $1000s.

### Method

<img src="/E2FAB9C2-F07C-4144-8C37-AF6C46FDD7CA.jpeg" width="400" height="300">

After cleaning the Boston dataset and exploring the predictors' relationship with the mystery response variable, it was found that 10 observations were missing from the response variable. However, upon analysis, it was determined that these omissions appeared to be random, as there was no significant difference in the means of the predictor variables between observations with missing responses and those with recorded responses. Consequently, the decision was made to omit these observations without responses, resulting in a dataset containing 496 total observations. Further examination involved plotting each predictor against the response variable to identify any concerning relationships. This comprehensive approach allowed for a thorough understanding of the dataset's structure and paved the way for subsequent model building and analysis.

<img src="/E29D7A47-2560-47D1-82B5-13603DDAC09F.jpeg" width="400" height="300">

An exploratory data analysis (EDA) was conducted on the Boston housing dataset. Initially, the data was loaded, checked for missing values, and explored through summary statistics. Ten missing values were identified in the response variable, "Resp," which were then isolated and examined. It was determined that these missing values appeared to be random. To proceed with the analysis, the rows with missing values were removed, ensuring the dataset was complete. Means and standard deviations were calculated for each variable before and after removing missing values to understand their distributions. The exploratory analysis included visualizations such as scatter plots of each feature against the response variable to identify potential relationships. Correlation Analysis was conducted.


Various linear and non-linear models were implemented and evaluated using the Boston housing dataset. Initially, the data was divided into training and test sets, and linear models were fitted using different methods such as least squares, ridge regression, lasso regression, principal component regression (PCR), and partial least squares (PLS) regression. Additionally, non-linear models including bagging, random forest, and boosting were applied to the data. The performance of each model was assessed using mean squared error (MSE) on the test set. Among the linear models, the best performance was achieved by the least squares model, while bagging yielded the lowest MSE among the non-linear models. Furthermore, cubic splines, natural splines, and smoothing splines were employed with the predictor variable "medv" to explore potential improvements in model performance, but these approaches did not outperform the best-performing models from earlier analyses. Overall, this comprehensive analysis provides insights into the effectiveness of different modeling techniques for predicting housing prices in Boston.

### Conclusion
In conclusion, this analysis of various linear and non-linear modeling techniques on the Boston housing dataset has provided valuable insights into the predictive performance of different methodologies. The experimentation revealed that among the linear models, least squares regression exhibited competitive performance, while bagging emerged as the most effective non-linear model in terms of minimizing mean squared error on the test set. Despite exploring the potential of splines with the predictor variable "medv," these techniques did not surpass the performance of the top-performing models. This study underscores the importance of thorough model evaluation and selection, as well as the need to consider both linear and non-linear approaches when tackling predictive modeling tasks. Moving forward, further exploration could involve refining model parameters, feature engineering, or incorporating additional variables to enhance predictive accuracy. Overall, this analysis serves as a foundation for future research and practical applications in the domain of housing price prediction.
