# Boosting_on_perf_multicoll
The following experiment was created to look at the behavior of several gradient Boosting Mechanisms, and how they deal with a a perfect multicollinearity, that 
is induced from 100 % copied features. Results indicate that the EBM as a bagging Boosting / Generalized Additive Model delivers mostly the same impact of all collinear features on a target, while the rest will be attributed to a constant.
Other methods do not give the three identical features an identical contribution. This may be bad or good depending on the situation. For further information see here:
https://stats.stackexchange.com/questions/550499/how-shap-values-behave-in-terms-of-multicollinearity-in-trees-ensemble-gradien