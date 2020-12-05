# ml_models_benchmark

Comparing different ML models on two regression and two classification problems including numeric and categorical features as well

1. Dataset 1: Predicting diamond prices by 6 input features - 3 categorical, 3 numerical
    -  X: (1) carat, (2) clarity, (3) color, (4) cut, (5) table and (6) depth
    - y: diamond price
    - download from: https://www.kaggle.com/shivam2503/diamonds

2. Dataset 2: Predicting laptop prices by 11 input features - 6 categorical, 5 numerical
    - X: company, type,	inches,	cpu,	gpu,	op_sys,	touch_screen,	hd_category,	ram	memory_SSD,	memory_HDD,	weight
    - y: laptop price
    - download from: https://www.kaggle.com/ionaskel/laptop-prices    
    
3. Dataset 3: Classifying bank customers into ones who do subscribe to long term deposits and to ones who do not (6 feautures - 3 num, 3 cat)
    - X: age, marital status, job status, education, has home loan, has personal loan
    - y: classes 1 (subscriber) and 0 (non subscriber)
    - download from: https://www.kaggle.com/raosuny/success-of-bank-telemarketing-data
  
ML models tried out
  1. dummies
  2. neighbors (KNN, RNN)
  3. regressions (penalized and unregularized)
  4. support vector machines (linear, polynomial and radial basis)
  5. decision tree
  6. random forest
  7. boosted trees: AdaBoost, GradientBoostingMachine, xgBoost, LightGBM, CatBoost

Winners

1. **Diamonds**: CatBoost by a small margin

    <img src="https://camo.githubusercontent.com/978ad57e1fba31f89403bdc139b9dbaffe70d32e88e31e4017897d902955dcad/687474703a2f2f73746f726167652e6d64732e79616e6465782e6e65742f6765742d646576746f6f6c732d6f70656e736f757263652f3235303835342f636174626f6f73742d6c6f676f2e706e67" width="300">

    Came very close: LightGBM, simple gradient boosting machine, xgBoost and random forest

    Overall scoreboard:
    
    
    <img src="https://github.com/kristofrabay/ml_models_benchmark/blob/main/notebooks/diamonds/scoreboard.png" width="750">


2. **Laptops**: xgBoost by a small margin 

    <img src="https://upload.wikimedia.org/wikipedia/commons/6/69/XGBoost_logo.png" width="250">


    Came very close: CatBoost, LightGBM

    Overall scoreboard:
    
    
    <img src="https://github.com/kristofrabay/ml_models_benchmark/blob/main/notebooks/laptops/scoreboard.PNG" width="750">
    
    
3. **Banks**: Simple Gradient Boosting Machine from sklearn API

    <img src="https://miro.medium.com/max/439/1*TN3K15kcQUDYPsl8SM5DcA.png" width="200">

    Came very close: xgBoost, Random Forest

    Overall scoreboard:
    
    
    <img src="https://github.com/kristofrabay/ml_models_benchmark/blob/main/notebooks/bank/scoreboard.PNG" width="750">
