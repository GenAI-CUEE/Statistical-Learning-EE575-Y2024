### Tutorial 5: Support vector machine
 
To support `Lecture 12: Support vector machine` ...  by *Suwichaya Suwanwimolkul, Ph.D.*


### HW 4. Support vector machine
#### Goal: 
  - can implement SVM and train the model.
  - can use the evaluation metrics and validation techniques for choosing the best configuration of the hyperparameters in SVM.  

#### Assignment sheet  

Download the [Google doc: Lab4](https://docs.google.com/document/d/1lWBvb9OQFmyp9sb9t6UMkYqNuXfTGSRJpQ4XxbNP_WY/edit?tab=t.0) and answer all the questions. 


- 1. Explain how you set up the experiment, e.g., 
  - a. How you split the data for training, validation, and testing.  
  - b. Find out the default hyperparameter setting for each kernels,
  - c. Declare which assessment metric that you use to check SVM’s performance (e.g., F1-score, accuracy, ROC curve). 
  - You can do this by using a diagram or flowchart to help explain.

- 2. Finding the suitable kernel. Show how the learned model has changed with different kernels: 
  - a. Linear kernel (`linear`)
  - b. Polynomial (`poly`) 
  - c. Radial basis function (`rbf`) 
 
- 3. Find the most suitable kernels based on the performance on the validation dataset.
  - a. The plot of the SVM performance curves versus different kernels.  You need to use the validation dataset to verify SVM performance. 
  - b. Show the scatter of validation data points against the decision contours across different kernels. Note that you should use the training data for showing the decision contours. 
  - c. Explain which decision contour that you would choose to fine-tuning the results.  


- 4. Fine-tuning phase.   
  You have to implement your own python script to perform fine-tuning.  
  - a. Explain how you set up the experiment for fine-tuning.  
    - Declare how you will adjust the hyperparameter setting for the chosen kernels.  
    - Declare how you will verify if the fine-tuning performance is getting better. 
  - b. The plot of the SVM performance curves versus different hyperparameter settings.  You need to use the validation dataset to verify SVM performance. 
  - c. Explain which hyperparameter setting is the best for the chosen kernels. 
  - d. Verify if the final setting gives the best performance on testing data.  

Make sure that every point that you made is supported by the evidence and the data.
