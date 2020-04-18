# Group assignment on Kaggle 
by

- Ibra Lujumba
- Tindi Kester Bevin Batariganya 
- Baker Lwasampijja

In predicting housing prices from the dataset, we used the worflow below to achieve our goal

## Plan of action <br/>

### Exploratory Data Analysis (EDA)
This was aimed at trying to understand the structure of the data and features that it contains.
In this step, the extent of missingness of the data in the features is known and strategies for downstream analysis are made. Correlations between features, distributions of the features and data type of each feature.

### Data cleaning and Missingness imputation
To remove features whose data is sparse and also fill up any missing data in features where the missing data was below the pre-defined threshold. The threshold set was 'any feature with more than 30% of the data missing, this feature wass dropped.'

### Encoding categorical variables
Machine learning algorithms expect data in numeric form. Data that was in form of strings was encoded into numeric values.

### Outlier removal
Linear regression algorithms are affected by outliers which leads to a bias in their predictions. The model created does not generalize well with the data. This can be avoided by removing outliers that may cause such an effect.

### Feature engineering
The features in the data were transformed into other features that could better explain the underlying problem to the model to be used. This involved summing some of the features, creating boolean features and replacing some features as well as multiplication between features.

### Scaling
Since all features were not on the same, the values were scaled to bring them to a common scale. This has the advantage that it improve model predictions since no feature is taken as being more important to the predictions by virtue of having large values. Without scaling, such features are assigned higher weights in the resultant model.

### Modeling with Cross-Validation and Hyperparameter tuning
Rather than split into training and testing sets, cross-validation was used. Cross-validation is recommended for datasets where the number of featutres is many. This prevents the model from overfitting the data and creation of a more generalisable model that can be used for predicting on new data

Multivariate regression models in the sci-kit learn, xgboost and lightgbm libraries were used. These include;
- Linear regression
- Lasso regression
- Ridge regression
- Kernel ridge regression (ridge regression with kernel trick)
- Stochastic gradient descent
- ElasticNet
- GradientBoostingRegressor
- RandomForestRegressor
- XGBoost
- LightGBM regressor
- Epsilon-Support Vector Regression

### Deep Learning Techniques
Neural networks from the tensorflow/keras library were also used in predicting housing prices.