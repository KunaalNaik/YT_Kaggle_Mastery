# Objective : Solve 5 Projects on Kaggle (Tabular Data)

## Five Problem Statements

1. **Classification** 
	- Spaceship Titanic: https://www.kaggle.com/competitions/spaceship-titanic
	- Algorithm: [sklearn Logistic Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)
2. **Regression** 
	- House Prices: https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques
	- Algorithm: [sklearn Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html#sklearn.linear_model.LinearRegression)
3. **Clustering** 
	- Mall Customers: https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python
	- Algorithm: [sklearn Cluster](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html?highlight=kmeans#sklearn.cluster.KMeans)
4. **Forecasting** 
	- Store Sales Forecasting: https://www.kaggle.com/competitions/store-sales-time-series-forecasting
	- Algorithm: [skforecast](https://github.com/JoaquinAmatRodrigo/skforecast)
	- Resource: [Skforecast](https://www.cienciadedatos.net/documentos/py27-time-series-forecasting-python-scikitlearn.html)
5. **Text Classification** 
	- Disastor Tweets: https://www.kaggle.com/competitions/nlp-getting-started
	- Algorithm: [sklearn Ridge Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Ridge.html)
	- Other Package: [sklearn Feature Extraction](https://scikit-learn.org/stable/modules/feature_extraction.html)

## Execution Framework

1. Follow CRISP-DM framework
2. End to End with Solution: Make One Submission per session
3. Write solution with all basic methods 
4. **Set Goals & Intent**
	1. Guideline - 1 x 2 x 3 Method
		- 1 Problem Statement
		- 2 hours per day 
		- 3 times per week
5. Make a Reoccuring meeting with yourself
	- Use Google Calendar

## How to write solutions?

1. **Iteration1**: Base solution
	1. Base solution first 
		- Import Train and Test Data
		- Check Data Types, ID's and Target columns
		- Divide Data into X and y
		- Identify Numerical and Categorical Columns
			- Drop columns with other data types for the first iteration
		- Missing Values
			- Identify
			- Numerical - treat with Median
			- Categorical - treat with Constant Strategy (fill N/A with "Missing")
		- Encode Categorical
			- Identify Text based columns
			- Create dummies using One Hot Encoding
		- Build a Model
		- Check Accuracy
		- Create Submission File
2. **Iteration2**: Validation Strategy
	1. Introduce Train Test Validation Strategy
		- Divide Data into Train and Validation - Test % - 33%
		- Build Model using Train
		- Evalute Train and Test Accuracy
		- Check for Overfitting/Underfitting
3. **Iteration3**: Outlier Treatment
	1. Introduce Quartile Outlier Treatment
		- Identify features with Outliers using Box Plot
		- Calculate Q1 & Q3
		- Calculate IQR
		- Calculate Upper and Lower Whisker
		- Treat Outliers
4. **Iteration4**: Tranformation
	1. Introduce Numerical Transformation
		- Identify Non-Normal features using Hist Plot
		- Transform features using StandardScaler
5. **Iteration5**: Feature Selection
	1. Introduce Feature Selection 
		- Use SelectKbest to select top features for modelling
6. **Iteration6**: Feature Importance
	1. Calculate which features are the most important
		- Create Column Names and Feature Importance Dataset
		- Plot Top 10 Feature Importance
		- Export Top Feature Plots
7. **Analyse Outcomes**:
	1. Analyse the predictions
	2. Make it consumable by business

