Notes: 
(1) updated a lot of libraries in requirements.txt file because it would break the pipeline due to old dependencies 
(2) installed cmake which xgboost and lightgbm rely on 
    Did the following through this statement: 
    - brew install cmake
    - cmake --version # checks version for you 
    - which cmake # where it is located 

(3) zenml breaking because it depends on distutils which causes a break 
    - solution 1: change zenml version >=0.66