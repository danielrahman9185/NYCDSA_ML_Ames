README -- Housing Price Prediction Project
Authors: Daniel Rahman & Steven Lee 

Introduction
The purpose of this project is to create a machine learning model that can accurately predict a house's sale price. 

Dataset
The dataset comes from a Kaggle competition dataset. The dataset includes sale price & 79 house/property variables for homes in Ames, Iowa. The explanatory variables in the dataset shed light on characteristics such as house/property size, house condition/characteristics, information on features such as basements and pools, and information such as year remodeled. 


I. EDA 

One of the first things that we noticed from the distribution of the dependent variable, sales price, is that it's right skewed. We examined its log transformation and saw that it was more normal/Gaussian. 

We then conducted EDA on the relationship between sales price and the explanatory variables. We first noticed, as one would intuitively believe, that both house area and living conditions are important in determining the house. We saw that the top three variables correlated with 'SalePrice' are 'OverallQual' and two area variables ('GrLivArea' & 'TotalBsmtSf').  
 

We also explored the presence of outliers -- we could see some clearly on the initial scatterplots that we graphed. We removed some outliers for numerical variables that deviated more than 6 stdev's from the mean. 



III. Data Preprocessing 
We had to examine and preprocess the dataset prior to beginning any modeling. Many of the variables had missing or NaN values which we had to manipulate through imputation. The categorial variables had more missing values than numeric. Next, we created ordinal values for the ordinal categorical variables.


IV. ML
We created linear regression and tree based models, testing MLR, Ridge, Lasso, Elastic Net, Random Forest, and Gradient Boost. Our two best performing models were Gradient Boost and Ridge. 
