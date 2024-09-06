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
Training Results:
The mean absolute error, or MAE, is 2.03e-08, or nearly zero.
The mean square error, or MSE, is 9.38e-16, or nearly zero.
R-squared: 1.0, or an ideal match
Test Results: MSE: 3,563,431,481.14; MAE: 50,452.16
9999982061520049 is the R-squared.
An R-squared of 1.0 indicates that the Linear Regression model overfits the data, capturing noise and patterns unique to the training set instead of adapting effectively to new, unknown data. However, the model did fit the training data flawlessly.

2. Linear Regression
