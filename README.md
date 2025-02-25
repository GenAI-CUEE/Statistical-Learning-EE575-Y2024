 Our goal is to provide the code-based visualization and exercises to understand the mathematics behind each of lectures in **Statiscal Learning EE2102575** by *Suwichaya Suwanwimolkul*.


This class is taught at Chulalongkorn University (EE575).  
You can find the records (in Thai) provided in the [video list (Youtube)](https://www.youtube.com/playlist?list=PLYrwEv08Hccg2POIP2l7e99xM9DzHDrS9). 

Lecture notes are provided in [this Google drive](https://drive.google.com/drive/folders/19ORjfJ2XGgyTfBRMBhfc8811DtU6S0M4?usp=sharing).
 


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

  - To implemention of OLS (Linear regression)
  - Perform model selection (AIC, AICs, BIC, cross-validation)
  - Then, implement k-fold cross validation
  - Docs:     
    - [How to calculate model selection scores (AIC, AICs, BIC, R2...)](Lab1/model_selection.ipynb)  
    - [HW 1: linear regression and model selection (AIC, AICs, BIC, cross-validation)](Lab1/main.ipynb) 
    

- [x] [Lab 2: Robust regression and regularization](Lab2/readme.md) 

  - To study about indentifying outliers and outlier analysis. [Lab 2: Outlier diagnostics](Lab2/outlier_diagnostics.ipynb)  provides two outlier analyses.

    - H-matrix    
    - Cook's distance  

  - Complete all the questions in the lab report provided in [Google doc Lab2](https://docs.google.com/document/d/1-dJQiSUfh7xgOnS_mmyO56fu2aH97bs2UKa3ktmkDko/edit?usp=sharing)


- [x] [Lab 3: Classification task using logistic regression and neural network](Lab3/readme.md)  
 
  - To study about how early stopper works in [logistic regression notebook](logistic_regression.ipynb).     
  - For [main notebook](Lab3/main.ipynb), we provide a training script for neural network with early stopper.    
      - Explain how you will extend this notebook to select the number of layers, e.g., 1, 2, 3.     
      - Provide F1 / BCE loss curves versus the number of layers. 
      - Show how to select the number of layers using the F1 / BCE loss curves vs. the number of layers.    
      - Provide your answer here [Google doc Lab3](https://docs.google.com/document/d/1Yd3etwo5Di_udjXMxGutus34x6QzpV8Q-hruVncHNnY/edit?usp=sharing)


- [x] [Midterm example](Midterm_example/Readme.md)  
 
  -   You will find the necessary information and Python tools within the provided Jupyter notebook to answer the questions in this lab:  [Jupyter notebook](Midterm_example/main.ipynb) or <a target="_blank" href="https://colab.research.google.com/github/GenAI-CUEE/Statistical-Learning-EE575-Y2024/blob/master/Midterm_example/main.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>  
  
  - The questions are provided in [Midterm example](Midtermexample_year2025.pdf)
    
    In this, you will be tasked to 
  
    - Answering some quizzes about feature correlation, logistic regression, kNN, LDA, and QDA  
    
    - Implementing the logistic regression, kNN, LDA, and QDA  
    
    - Making analysis of the results and evaluation such as confusion matrix, precision-recall, etc. 
    
    - Then use the results to answers the questions (example questions are provided in the Midtermexample_year2025.pdf). 
 