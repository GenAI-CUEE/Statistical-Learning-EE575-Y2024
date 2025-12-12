 Our goal is to provide the code-based visualization and exercises to understand the mathematics behind each of lectures in **Statiscal Learning EE2102575** by *Suwichaya Suwanwimolkul*.

 
### HW 3. Logistic regression and neural network  
#### Goal: 
  - can implement and train a neural network.
  - can use the evaluation metrics and validation techniques for choosing the best configuration of neural network. 
  - understand how to use early stopper. 
   
#### Assignment sheet
  
Download the [Google doc: Lab3](https://docs.google.com/document/d/1Yd3etwo5Di_udjXMxGutus34x6QzpV8Q-hruVncHNnY/edit?tab=t.0) and answer all the questions. \

Please download it as a PDF file and rename it from `Lab3.pdf` to `Lab3_G1.pdf`. 

- Q1. Explain how early stopper works. You can do this by providing the flowchart and use the example in the ipnb: [logistic regression notebook](logistic_regression.ipynb) or <a target="_blank" href="https://colab.research.google.com/github/GenAI-CUEE/Statistical-Learning-EE575-Y2024/blob/master/Lab3/logistic_regression.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>     

- Q2. Explain how you will extend the neural network and select the different neural network configurations using validation technique. 
  - a. Provide the code to extend the number of layers to 1, 2, 3. 
  - b. Plot F1 / BCE loss curves versus the number of layers. Then, explain which you would use. 
  
  The code is implemented in [main notebook](main.ipynb) or     
    <a target="_blank" href="https://colab.research.google.com/github/GenAI-CUEE/Statistical-Learning-EE575-Y2024/blob/master/Lab3/main.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>  
    
    This notebook already provided: 
      - Tools and packages
      - Download student depression dataset from [kaggle](https://www.kaggle.com/datasets/hopesb/student-depression-dataset) 
      - Data processing
