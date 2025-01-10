 Our goal is to provide the code-based visualization and exercises to understand the mathematics behind each of lectures in **Statiscal Learning EE2102575** by *Suwichaya Suwanwimolkul*.

### Environments

- Create and install conda environment \
  `conda create -n EE575`  
  `conda activate EE575` 
  `conda install pip`
- Install required packages \
  `pip install -r requirements.txt`  

### Topics

The coding scripts & excercises are 

- [x] [Lab 1: linear regression and model selection (AIC, AICs, BIC, cross-validation)](Lab1/readme.md) 

  - Data processing
    - Data reading and preprocessing
    - Data splitting
    - Data normalization
    - Visualizing data correlation
  - Implemention of OLS (Linear regression)
  - Perform model selection (AIC, AICs, BIC, cross-validation)
  - Implement k-fold cross validation
  - Docs:     
    - [How to calculate model selection scores (AIC, AICs, BIC, R2...)](Lab1/model_selection.ipynb)  
    - [HW 1: linear regression and model selection (AIC, AICs, BIC, cross-validation)](Lab1/main.ipynb) 
    

- [x] [Lab 2: Robust regression and regularization](Lab2/readme.md) 

  - Complete 2 outlier analysises: [Lab 2: Outlier diagnostics](outlier_diagnostics.ipynb) <a target="_blank" href="https://colab.research.google.com/github/GenAI-CUEE/Statistical-Learning-EE575-Y2024/blob/master/Lab2/outlier_diagnostics.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
        </a>

    - H-matrix    
    - Cook's distance  

  - Complete all the questions in the lab report provided in [https://docs.google.com/document/d/1-dJQiSUfh7xgOnS_mmyO56fu2aH97bs2UKa3ktmkDko/edit?usp=sharing]


- [x] [Lab 3: Classification task using logistic regression and neural network](Lab3/readme.md)  

 