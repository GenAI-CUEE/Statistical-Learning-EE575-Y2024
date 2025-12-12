 Our goal is to provide the code-based visualization and exercises to understand the mathematics behind each of lectures in **Statiscal Learning EE2102575** by *Suwichaya Suwanwimolkul*.


### HW 2.  Outlier analysis and regularization 
#### Goal: 
  - can implement two outlier analysises: H-matrix and Cook's distance  
  - point out the differences between H-matrix and Cook's distance in the algorithm from a theoretical point of view. 

#### Assignment sheet

  - Download the [Google doc: Lab2](https://docs.google.com/document/d/1-dJQiSUfh7xgOnS_mmyO56fu2aH97bs2UKa3ktmkDko/edit?tab=t.0) and answer all the questions. \
    Please download it as a PDF file and rename it from `Lab2.pdf` to `Lab2_G1.pdf`. 

  - Q1. We have partially implemented a framework to find outliers. Your task is to complete the following functions: 
      - `H_matrix_leverage` that compute the H-matrix and find the diagonal elements in the matrix: $H = X (X^T X)^{-1} X^T$

      - `CookDistance` to compute the Cook's distance for all `j = 1 ... m` elements. 
   
      - The two outlier analysises are provided in [Lab 2: Outlier diagnostics](outlier_diagnostics.ipynb)   or     <a target="_blank" href="https://colab.research.google.com/github/GenAI-CUEE/Statistical-Learning-EE575-Y2024/blob/master/Lab2/outlier_diagnostics.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
      </a>. This notebook provides:   
          - Tools and packages
          - Download data from [kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data) 
          - Data processing 
          
  - Q2. Point out the differences between H-matrix and Cook's distance in the algorithm from a theoretical point of view. Mainly, you should be able to verify ...
    - Q2.a. Are the outliers identified by the two methods intersect?
    - Q2.b. Are there any outliers identified that have been chosen differently by each of the methods? 
    - Q2.c. How is the performance improved by removing the outliers identified by H-matrix versus the Cook's distance ? 
    
  - Please answer these questions using your results in Lab2 to provide the discussion. Make sure that every point that you made is supported by the evidence and the data.