#### property-values

### Project Goal
Build models to predict property values in Bexar County

### Summary
The data set included 608 properties with attributes and values and 5 properties with attributes and without values. Based on Bexar County Appraisal District data, the 29 variables provided were defined, cleaned, and explored. Multiple types of regression models were run in order to predict home values, including: OLS (Ordinary least squares), GLM (generalized linear model), random forest, GAM (generalized additive model), SVM (support vector machine), and MARS (multivariate adaptive regression splines, using earth). First, the models were run with all available predictors and because of the presence of degenerate variables, likely resulting in unstable models. The degenerate variables were removed and the models were run with 12, 11, and 10 predictors. The variation in total predictors is due to high correlation between variables.

### Results
Ultimately, the earth model produced the best predictions with 11 predictor variables and a test RMSE of $8,472.24, approximately 4% of the median home value of the 605 observations. The actual error, based on the actual home values provided after the completed exam, was off by an average of $5,334.20.

RMSE was used as a performance metric because there were unexpected values, potential outliers, that needed to be considered. Another benefit of using RMSE is maintaining the units of the original data, in this case, dollars.

### Included
R script, predictions, actual values

### Programs
R (dplyr, ggplot2, caret, AppliedPredictiveModeling), lattice, corrplot, pls, elasticnet, reshape2, RANN, Hmisc, gam, e1071, NbClust)

### Additional Information
Course: Data Analytics Applications
