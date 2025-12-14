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

- [x] [HW 1. Linear regression and model selection (AIC, AICs, BIC, cross-validation)](Lab1/readme.md) 
  - Goal:
    - can implement cross-validation for training a model.
    - see the difference between cross-validation and hold-out method.
    - can apply the evaluation scores for selecting the best configuration for a linear regression model.
    

- [x] [HW 2.  Outlier analysis and regularization](Lab2/readme.md) 

  - Goal 
    - can implement two outlier analysises: H-matrix and Cook's distance  
    - point out the differences between H-matrix and Cook's distance in the algorithm from a theoretical point of view. 


- [x] [HW 3. Logistic regression and neural network](Lab3/readme.md)  
  - Goal
    - can implement and train a neural network.
    - can use the evaluation metrics and validation techniques for choosing the best configuration of neural network. 
    - understand how to use early stopper. 


- [x] [HW 4. Support vector machine](Lab4/readme.md)  
  - Goal
    - can implement SVM and train the model.
    - can use the evaluation metrics and validation techniques to choose the best model configuration for SVM.

- [x] [HW 5. Clustering algorithms](Lab5/readme.md) 
  - Goal
    - can implement and configure the clustering algorithms.
    - can provide the reasons why the chosen algorithm is the most suitable for given datasets. 
    - can provide the answer with evidence.


- Others
  - [x] [Decision-tree tutorial](Lab5/readme.md)  
        Building tree is a greedy approach to select the feature space partitioning. In this exercise, we hope that you can learn how the decision tree is built.    
        In fact, we have adopted the implementation from [Normalized nerd](https://www.youtube.com/@NormalizedNerd). 
        So, feel free to watch the video: [Decision tree for regression](https://www.youtube.com/watch?v=UhY5vPfQIrA), as your reference. 
    
      - Your tasks are 
        1. Provide the flowchart for `build_tree(self, dataset, curr_depth=0)` in the `DecisionTreeRegressor class`. 
        - We have provided the flowchart in [Lab4.drawio](Lab5/FlowChart/Lab4.drawio), but the flow chart is incomplete. You can open this file via [https://app.diagrams.net/](https://app.diagrams.net/). 
        - Please provide an explanation of your flowchart in [the lab sheet report](https://docs.google.com/document/d/1k8ZRV82h77Vwxc1H-u_OzqdHPrGLDGJwGSPyFx42M9M/edit?usp=sharing). [Reference. https://www.geeksforgeeks.org/unified-modeling-language-uml-introduction/](https://www.geeksforgeeks.org/unified-modeling-language-uml-introduction/)

        2. If one has to modify this implementation for classification task, which functions in [Decision tree class](#decision-tree-regressor-class) should be changed? Please provide your reason in [the lab sheet report](https://docs.google.com/document/d/1k8ZRV82h77Vwxc1H-u_OzqdHPrGLDGJwGSPyFx42M9M/edit?usp=sharing). 


  - [x] [Midterm example](Midterm_example/Readme.md)  
  
    -   You will find the necessary information and Python tools within the provided Jupyter notebook to answer the questions in this lab:  [Jupyter notebook](Midterm_example/main.ipynb) or <a target="_blank" href="https://colab.research.google.com/github/GenAI-CUEE/Statistical-Learning-EE575-Y2024/blob/master/Midterm_example/main.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>  
    
    - The questions are provided in [Midterm example](Midtermexample_year2025.pdf)
      
      In this, you will be tasked to 
    
      - Answering some quizzes about feature correlation, logistic regression, kNN, LDA, and QDA  
      
      - Implementing the logistic regression, kNN, LDA, and QDA  
      
      - Making analysis of the results and evaluation such as confusion matrix, precision-recall, etc. 
      
      - Then use the results to answers the questions (example questions are provided in the Midtermexample_year2025.pdf). 