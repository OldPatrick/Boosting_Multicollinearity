# Behavior of several Boosting Algorithms on Multicollinearity (identical features in this case)
The following experiment was created to look at the behavior of several gradient Boosting Mechanisms, and how they deal with a a perfect multicollinearity, that 
is induced from 100 % copied features. Experiment was set up with these 8 Boosting Regressor Methods:

<b>sklearn package:</b>
DecisionTreeRegressor, RandomForestRegressor, ExtraTreesRegressor, GradientBoostingRegressor
<br>

<b>other packages:</b>
CatBoostRegressor , ExplainableBoostingRegressor , LGBMRegressor, XGBRegressor

Results indicate that the EBM as a bagging Boosting / Generalized Additive Model delivers mostly the same impact of all collinear features on a target, while the rest will be attributed to a constant, while exmaining the shap values/ebm importances over 2000 random seeds.
Other methods do not give the three identical features an identical contribution. This may be bad or good depending on the situation. For further information see here:
https://stats.stackexchange.com/questions/550499/how-shap-values-behave-in-terms-of-multicollinearity-in-trees-ensemble-gradien
