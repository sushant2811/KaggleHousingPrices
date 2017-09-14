# KaggleHousingPrices

Jupyter notebook for housing prices prediction competition on Kaggle. 
The training data consists of 1460 houses and 79 features describing the houses 
in Ames, Iowa which is then used to predict house prices for the test data.

The training data is cleaned and processed to indentify the most relevant 
features and correct for skewness.  After appropriate imputation and feature 
selection, the machine learning models are trained. 
Since, we have a mix of categorical and continuous features (and there are a 
large number of them), we use the ensemble methods---Random Forest and 
Gradient Boosting---which are known to generally 
perform well.  Through cross validation, we find that the Gradient Boosting 
does slightly better than Random Forest and we use it to make predictions on 
the test data.  

Kaggle submissions are evaluated on Root-Mean-Squared-Error (RMSE) between the 
logarithm of the predicted value and the logarithm of the observed sales price. 
Our model receives a score of 0.132. (The 10th place score is 0.113)



