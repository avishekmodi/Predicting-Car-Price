# Predicting-Car-Price
Creating a model that predicts the Price of used cars.
At first the data is cleaned as the raw data contains too much noises for a proper predicting capability.
After cleaning of the data, Exploratory Data Analysis is done, check for outliers, check for Nan values and replace them, if any, with median values, various relationships between the different features/columns(independet variables) and the target/dependent feature is seen to gain some knowledge about them.
Since the number of features is less so we do not remove any of the feature from the dataset even if two of the features have a very high correlation among them it is done so we do not lose some important feature.
After the EDA, One Hot Encoding is done for categorical features (and to avoid the dummy varuable trap we do drop_first=True) 
Since the problem is Regression problem statement I make use of Linear Regression, since the Linear Regression is easily interpreted and properly shows the marginal changes in the independent variables(predictors) and observed their consequences on the dependent variable(response)
Now, I make use of a Pipeline which takes the raw traing data from one side and then perform the Ohe(One Hot Encoding) to the categorical data while passing the non categorical features and then will fit the Linear Regression. This use of pipeline makes the fitting of model quite easy.
