# ml_models_benchmark
Comparing different ML models on a simple regression problem including numeric and categorical features as well

Dataset: Predicting diamond prices by 6 input features - 3 categorical, 3 numerical
  - X: (1) carat, (2) clarity, (3) color, (4) cut, (5) table and (6) depth
  - y: diamond price
  
ML models tried out
  1. dummy regressors
  2. neighbors (KNN, RNN)
  3. regressions (penalized and unregularized)
  4. support vector machines (linear, polynomial and radial basis)
  5. decision tree
  6. random forest
  7. boosted trees: AdaBoost, GradientBoostingMachine, xgBoost, LightGBM, CatBoost

Winner: CatBoost by a small margin

![CatBoost](https://camo.githubusercontent.com/978ad57e1fba31f89403bdc139b9dbaffe70d32e88e31e4017897d902955dcad/687474703a2f2f73746f726167652e6d64732e79616e6465782e6e65742f6765742d646576746f6f6c732d6f70656e736f757263652f3235303835342f636174626f6f73742d6c6f676f2e706e67)

Came very close: LightGBM, simple gradient boosting machine, xgBoost and random forest

Overall scoreboard:

