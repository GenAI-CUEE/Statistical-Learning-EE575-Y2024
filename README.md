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

- [x] [Lab 4. SVM](Lab4/readme.md)  
    In this tutorial, we will build SVM for binary-class classification. 
    - In this experiment, we will investigate 
      1. how the learned model has changed as the regularization parameter $C$ increased or decreased ( C = 1000 vs. C = 0.001)... This can be explained by showing the differences in the support hyperplanes and the target hyperplane. 
      
      2. how the performance on the test data looks like as the regularization parameter $C$ increased or decreased 

      You can provide your results in the lab sheet: [the lab sheet report](https://docs.google.com/document/d/1lWBvb9OQFmyp9sb9t6UMkYqNuXfTGSRJpQ4XxbNP_WY/edit?usp=sharing)   


- [x] [Lab 5. Decision tree ](Lab5/readme.md)  
      Building tree is a greedy approach to select the feature space partitioning. In this exercise, we hope that you can learn how the decision tree is built.    
      In fact, we have adopted the implementation from [Normalized nerd](https://www.youtube.com/@NormalizedNerd). 
      So, feel free to watch the video: [Decision tree for regression](https://www.youtube.com/watch?v=UhY5vPfQIrA), as your reference. 
  
    - Your tasks are 
      1. Provide the flowchart for `build_tree(self, dataset, curr_depth=0)` in the `DecisionTreeRegressor class`. 
      - We have provided the flowchart in [Lab4.drawio](Lab5/FlowChart/Lab4.drawio), but the flow chart is incomplete. You can open this file via [https://app.diagrams.net/](https://app.diagrams.net/). 
      - Please provide an explanation of your flowchart in [the lab sheet report](https://docs.google.com/document/d/1k8ZRV82h77Vwxc1H-u_OzqdHPrGLDGJwGSPyFx42M9M/edit?usp=sharing). [Reference. https://www.geeksforgeeks.org/unified-modeling-language-uml-introduction/](https://www.geeksforgeeks.org/unified-modeling-language-uml-introduction/)

      2. If one has to modify this implementation for classification task, which functions in [Decision tree class](#decision-tree-regressor-class) should be changed? Please provide your reason in [the lab sheet report](https://docs.google.com/document/d/1k8ZRV82h77Vwxc1H-u_OzqdHPrGLDGJwGSPyFx42M9M/edit?usp=sharing). 