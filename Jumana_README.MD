Notes: 
(1) updated a lot of libraries in requirements.txt file because it would break the pipeline due to old dependencies 
(2) installed cmake which xgboost and lightgbm rely on 
    Did the following through this statement: 
    - brew install cmake
    - cmake --version # checks version for you 
    - which cmake # where it is located 