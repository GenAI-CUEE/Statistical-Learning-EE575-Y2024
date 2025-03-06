 Our goal is to provide the code-based exercises to understand the mathematics behind each of lectures in **Statiscal Learning EE2102575** by *Suwichaya Suwanwimolkul*.


### Decision tree  

  - [How to implement decision tree for regression tasks](main.ipynb) 
    
    <a target="_blank" href="https://colab.research.google.com/github/GenAI-CUEE/Statistical-Learning-EE575-Y2024/blob/master/Lab5/main.ipynb">
    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
    </a>

    This notebook provides: 

    - [Import tools](#import-tools)
    - [Get the data](#get-the-data) 
    - [Decision tree implementation](#decision-tree-implementation)
        - [Node class](#node-class)
        - [Decision tree class](#decision-tree-regresssor-class)
    - [Runing inference](#running-inference)
    - [sklearn's decision tree](#sk-learn-decision-treee-regressor)

    
    Building decision tree is a greedy approach to select the feature space partitioning in a tree. 
    Therefore, in this exercise, we hope that you can learn how the decision tree is built.    
    In fact, we have adopted the implementation from [Normalized nerd](https://www.youtube.com/@NormalizedNerd). 
    So, feel free to watch the video: [Decision tree for regression](https://www.youtube.com/watch?v=UhY5vPfQIrA), as your reference. 
 
  - Your tasks are 
    1. Provide the flowchart for `build_tree(self, dataset, curr_depth=0)` in the `DecisionTreeRegressor class`. We have provide the flowchart in [Lab4.drawio](Lab5/FlowChart/Lab4.drawio), but the flow chart is incomplete. Please provide an explanation of your flowchart in [the lab sheet report](https://docs.google.com/document/d/1k8ZRV82h77Vwxc1H-u_OzqdHPrGLDGJwGSPyFx42M9M/edit?usp=sharing). 

    2. If one has to modify this implementation for classification task, which functions in [Decision tree class](#decision-tree-regressor-class) should be changed? Please provide your reason in [the lab sheet report](https://docs.google.com/document/d/1k8ZRV82h77Vwxc1H-u_OzqdHPrGLDGJwGSPyFx42M9M/edit?usp=sharing).   

  - Your submitted files are:
    - [A lab sheet report](https://docs.google.com/document/d/1k8ZRV82h77Vwxc1H-u_OzqdHPrGLDGJwGSPyFx42M9M/edit?usp=sharing) 
      - to explain the flowchart for `build_tree`; and
      - to answer to the question of which functions in [Decision tree class](#decision-tree-regressor-class) should be changed so that the implementation will work for a classification task? 
    
    - To draw the flowchart for `build_tree`. You can do this by copying the provided flowchart and complete the missing flowchart in [Lab4.drawio](Lab5/FlowChart/Lab4.drawio). 

  - Always, set up your folder name as your group name, for example, "G1.zip"  (if you are in group no. 1) and submit it through `Assignemnts` (myCourseVille)