Problem Statement
Problem Type: Regression
Objective: The goal is to predict the Total value (total contribution from all activities) based on the different agricultural and non-agricultural activities, using the Sector and Nature of Operation as additional features.
Dataset source: data.gov.in
Dataset description: The dataset consists of 24 entries with 28 columns, which can be grouped into agricultural and non-agricultural activities. The dataset includes the following key components: 
1.Categorical Features:
  Sector: Describes the specific sector of the operation (e.g., Primary, Secondary, Tertiary).
Nature of Operation: Indicates the nature or type of operation within the sector (e.g., Private, Public, Cooperative).

2. Numerical Features:
Agricultural Activities:
 01 - Activities relating to agriculture other than crop production & plantation.
02 – Livestock.
03 - Forestry and Logging.
04 - Fishing and aqua culture
Subtotal: Agricultural Activities: Aggregates the agricultural activities.
Non-Agricultural Activities:
 05 - Mining and quarrying.
06 – Manufacturing.
07 - Electricity, gas, steam and air conditioning supply
08 - Water supply, sewerage, waste management and remediation activities
09 - Construction
10 - Wholesale trade, retail trade & repair of motor vehicles & motor cycles.
 11 - Wholesale trade .
12 - Retail trade.
 13 - Transportation and storage.
 14 - Accommodation and Food service activities.
15 - Information & communication.
16 - Financial and insurance activities.
17 - Real estate activities.
18 - Professional, scientific & technical activities.
19 - Administrative and support service activities
20 - Education
21 - Human health & social work activities.
22 - Arts entertainment, sports & amusement and recreation.
23 - Other service activities not elsewhere classified
    Subtotal: Non-Agricultural Activities: Aggregates the non-agricultural activities.
3. Target Variable:   
 Total: Represents the total contribution from all activities

Model Training and Regularization Techniques:
Initially, a Linear Regression model was trained utilizing a variety of parameters associated with both agricultural and non-agricultural activities in order to predict the target variable (Total). The disparity between the training and test performance measures indicates that this model overfitted despite performing very flawlessly on the training set.

1. The Linear Regression Method
The Linear Regression method was tested with a mean absolute error of 2.03e-08 and a mean square error of 9.38e-16, indicating that the model overfits the training data, capturing unique patterns instead of adapting effectively to new data.
2. Ridge Regression (L2 Regularization):
   Ridge Regression (L2 regularization) reduces overfitting by shrinking coefficients, making the model less complex. It slightly reduces R-squared value compared to Linear Regression, promoting trade-off between bias and variance.
3. Lasso Regression (L1 Regularization):
   Lasso Regression (L1 regularization) reduces overfitting and performs feature selection by adding a penalty to coefficients' absolute values. It achieves high R-squared values and potentially simplifies the model.
Results and Conclusions
   Linear Regression performed well on training data but showed overfitting. Ridge Regression reduced overfitting by applying L2 regularization and feature selection, making the model more robust to unseen data.
