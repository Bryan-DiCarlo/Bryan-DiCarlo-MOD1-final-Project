# Bryan-DiCarlo-MOD-1-Final-Project_v5
# Introduction
We will be investigating a publicly available data set containing house sale prices in King County in Washington State. This dataset contains house sale prices for King County, which includes Seattle. It includes homes sold between May 2014 and May 2015.  

* Develop a predictive model for house price that identifies housing features most closely assocciated with higher pricing 
* In line with this objective, we intend to formulate answers to some important questions that drive this investigation.  
 1. What housing features provide the most accurate prediction of sale price?  
 2. What effect does location have on a house's final selling price
 3. How does the size of a house relate to final selling price
 4. Will agressively marketing and showing your house result in a higher selling price
 5. What measures can the seller and agent take to maximize final selling price


* Our business goal is to develop a tool that quantitatively identifies housing features most closely associated with higher housing sales prices in King County.   A Tool that can be used by sellers and agents to provide recommendations for maximizing your sale price when listing your home in King County.

# MLR Model Summary and Evaluation
* The summary statistics describing our final model look very much like one would want with confirmation from two models
* R-squared value of 0.720 is substantial for the complexity of our data. This means that 72% of the variability in price can be accounted for with the five predictor variables included in our model
* Our coefficients are all positive as would we hope in this case.  The magnitude of each coefficient represents the increase in price per unit change in the predictor if all other factors are held constant.  We were looking for features that predict increasing price as the values of the predictors increase.  A positive relationship between the two. Our coefficients indicate this relationship.
* The p-values of the features are all zero.  This indicates our feature variables are statistically significant predictors of price. Meaning that the observed relationship between predictor and price happened by chance alone is virtually zero
* Our statistics describing the normality assumptions of our model are close to ideal. The skewness, kurtosis and JB statistic are all within acceptable limits of the ideal. This was greatly enhanced by log transforming several of our features used in our model.
* Anlysis of our Model's residuals shows they are evenly and normally distributed. Indicating our model is a good fit
* The RMSE gives us an indication of how close our predicted values of y are to the actual values of y from the data. Lower values of RMSE incate better fit. Our RMSE was 0.72 incating a good fit.
* Our biggest concern for our model is the presence of multicollinearity. The condition number is a measure of this effect.  From the first iteration of our model to the final iteration the condition was decreased on a scale from 10^19 to 10^4.  This still indicates some degree of collinearity
* That being said, the predictive power of our model is still unchanged.  This only affects the granularity and precision in which you can describe the contribution of each predictor variable.  Each variable may have some combined redundant affects in the model.
* Our ultimate business objective was to produce a tool for projecting housing prices in King county, Washington.  The model is unaffected in this regard

# Conclusion

We have developed an MLR model for predicting house prices in King County, Washington.  Our model does a solid job of predicting house prices.  The metrics used to a evaluate a Multiple Linear Regression all point to a good model. The most valuable outcome of our model, for our customers, is that we have identified 5 of the most import housing features related to increased sale price.

* They are, in order of importance:

 1. Location- as indicated by our Latitude feature
 2. Size- as indicated by our sqft_comb feature
 3. Waterfront - waterfront properties are worth more
 4. Grade - House with higher grades sell for more
 5. View - the number of times a house is viewed increases sale price
 
We have deloped a model that is a good predictor of housing prices in King County.  More importantly, in line with our business objectives, We have identified the the most relevant features for increasing a house's sale price.  We think this will be a valuable tool for seller and agent when trying to maximize your properties sale price.

# Future Directions: Take advantage of Geographical price clustering

# Notebook: Bryan DiCarlo MOD 1 Final Project_v5.ipynb

