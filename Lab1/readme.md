 Our goal is to provide the code-based visualization and exercises to understand the mathematics behind each of lectures in **Statiscal Learning EE2102575** by *Suwichaya Suwanwimolkul*.


### HW 1. Linear regression and model selection (AIC, AICs, BIC, cross-validation) 
#### Goal: 
  - can implement cross-validation for training a model.
  - see the difference between cross-validation and hold-out method.
  - can apply the evaluation scores for selecting the best configuration for a linear regression model.

#### Assignment sheet
  - Download the Google sheet and answer all the questions. \
    Please download them as a PDF file and rename it from `Lab1.pdf` to `Lab1_G1.pdf`. 

  - Q1. We have partially implement a cross-validation framework. Your task is to complete the function called `single_fold_operation`. You have to  
    - Q1.a. Write the flowchart and explain how the function `single_fold_operation` operated with other parts in the cross-validation framework which is in cell #9.    
    - Q1.b. Provide your code for `single_fold_operation` and explain what you have done. 

    The function `single_fold_operation` is provided in [main.ipynb](main.ipynb)  or
      <a target="_blank" href="https://colab.research.google.com/github/GenAI-CUEE/Statistical-Learning-EE575-Y2024/blob/master/Lab1/main.ipynb">
    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
    </a> 

      The details of `single_fold_operation` is as follows:  
        
      ``` 
      def single_fold_operation(train_X, train_y, train_subet_index, valid_subset_index)
        This function will perform the training and inference on the k-fold data. 
        Then, it will return the scores (AIC, AICs, BIC, AdjustedR2, RMSE_train, RMSE_valid)

        INPUTS: train_X, train_y, train_subet_index, valid_subset_index 
          train_X : an np.array containing the features of the training data
          train_y : an np.array containing the labels of the training data

          train_subet_index and valid_subset_index further subdivide the above training data for training and validation in a single fold. 

          train_subet_index: index set to select which data in train_X and train_y to be used for training the model.
          valid_subset_index: index set to select which data in train_X and train_y to be used for validating the model.
        
        OUTPUTS: scores  
          scores is a dictionary containing the following attributes {"AIC", "AICs", "BIC",  "AdjustedR2", "RMSE_train", "RMSE_valid"}  
      ``` 
      Hint! After getting `train_X, train_y, train_subet_index, valid_subset_index`, the function will run training and inference, in which you should get the predicted outcome of the training data (`y_train_pred`) and and the predicted outcome of the validation data (`y_valid_pred`).  
      
      Then, you may use `y_train_pred` and `y_valid_pred`  them to calculate the model selection scores...
                       
        ```
        train_subset = {"X":X_train_subset, "y":y_train_subset, "y_predict":y_train_pred}
        valid_subset = {"X":X_valid_subset, "y":y_valid_subset, "y_predict":y_valid_pred} 

        training_score = model_selection_scores(train_subset)
        valid_score   = model_selection_scores(valid_subset)
        ```
        # Then you may use these scores to provide the OUTPUT:  
        
          scores = {  "AIC": training_score["AIC"], 
                      "AICs": training_score["AICs"], 
                      "BIC": training_score["BIC"], 
                      "AdjustedR2": training_score["AdjustedR2"],
                      "RMSE_train": training_score["RMSE"], 
                      "RMSE_valid":valid_score["RMSE"] }

    
    
    Also, this notebook provides: 

    - Tools and packages
    - Download data from [kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data) 
    - Data processing 
    - Q1 is in cell #8
    - Show the averaged model selection scores: AIC, AICs, BIC, Adjusted R2 (using Training sets)
    - Show the averaged MSE scores from training and validation.
  
  - Q2. After you have finished the implementation, tell us which model is the best according to each selection scores: AIC, AICs, BIC, Adjusted R2 (using the training sets), and the averaged MSE scores (using the validation set).


  - Q3. Compare the above results with a hold-out validation. Tell us if you get the same conclusion for the best model using the averaged MSE scores (using the validation set).
  
    Here, we have prepare a python code for you for a hold-out validation: [hold_out.ipynb](hold_out.ipynb) or   
      <a target="_blank" href="https://colab.research.google.com/github/GenAI-CUEE/Statistical-Learning-EE575-Y2024/blob/master/Lab1/hold_out.ipynb">
      <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
      </a> . This notebook provides: 

    - [Tools-and-packages](#tools-and-packages)
    - [Data loading](#data-loading) from [Kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data) 
    - [Data processing](#data-preprocessing)
        - Data reading and preprocessing
        - Data splitting
        - Data normalization
        - Visualizing data correlation
    - [Implementing model (Linear regression or OLS)](#linear-regression-implementing-models)
    - [Compute AIC, AICs, BIC](#compute-aic-aics-bic-on-training-data)
    - [Performance on testing dataset (RSE, MSE)](#compute-performance-on-testing)
    - [Model selection AIC, AICs, BIC, Adjusted R2 (using Training data)](#model-selection-aic-aics-bic-adjusted-r2)