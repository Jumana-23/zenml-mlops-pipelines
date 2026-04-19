Notes: 
(1) updated a lot of libraries in requirements.txt file because it would break the pipeline due to old dependencies 
(2) installed cmake which xgboost and lightgbm rely on 
    Did the following through this statement: 
    - brew install cmake
    - cmake --version # checks version for you 
    - which cmake # where it is located 

(3) zenml breaking because it depends on distutils which causes a break 
    - solution 1: change zenml version >=0.66 (this didnt work)
    - solution 2: change python version to 3.11 (actually works and doesnt crash)

(4) merged cleanup-repo on main so that updated packages are now in main branch
(5) after installing zenml you will have a variable that you need to set to:
    - export OBJC_DISABLE_INITIALIZE_FORK_SAFETY=YES 
    this is so you can run the local server (terminal fix most likely will need to copy that statement above everytime you try to run local server)
    (5).a : issue was that dashboard was not running 
        - solution: brew install libomp 
