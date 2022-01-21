## Bank marketing Prediction Using Logistic Regression and Random-Forest
## Tasks to perform
Read in the file and get basic information about the data, including numerical summaries.

    i.Describe the pdays column, make note of the mean, median and minimum values. Anything
      fishy in the values?
      
    ii.Describe the pdays column again, this time limiting yourself to the relevant values of pdays. How
       different are the mean and the median values?
       
    iii.Plot a horizontal bar graph with the median values of balance for each education level value.
        Which group has the highest median?
        
    iv.Make a box plot for pdays. Do you see any outliers?
    
The final goal is to make a predictive model to predict if the customer will respond positively to the
campaign or not. The target variable is “response”.

First, perform bi-variate analysis to identify the features that are directly associated with the target
variable. You can refer to the notebook we used for the EDA discussion.

    i.Convert the response variable to a convenient form
      
    ii.Make suitable plots for associations with numerical features and categorical features’
      
    iii.Are the features about the previous campaign data useful?
      
    iv.Are pdays and poutcome associated with the target?
      
If yes, and if you plan to use them – how do you handle the pdays column with a value of -1 where the
previous campaign data is missing? Explain your approach and your decision.

Before the predictive modeling part, make sure to perform –

    i.The necessary transformations for the categorical variables and the numeric variables
    
    ii. Handle variables corresponding to the previous campaign
    
    iii.Train test split
    
Predictive model 1: Logistic regression
   i. Make a predictive model using logistic regression
   
   ii.Use RFE to select top n features in an automated fashion (choose n as you see fit)
   
   iii.Using p values and VIF, get rid of the redundant features
   
   iv.Estimate the model performance using k fold cross validation
   
   v. What is the precision, recall, accuracy of your model?
   
   vi.Which features are the most important from your model?
   
Predictive model 2: Random Forest

   i.Make a predictive model using random forest technique
   ii.Use not more than 50 trees, and control the depth of the trees to prevent overfitting
   iii. Estimate the model performance using k fold cross validation
   iv.What is the precision, recall, accuracy of your model?
   v.Using the feature importance values from the Random Forest module, identify the most
       important features for the model

Compare the performance of the Random Forest and the logistic model –
  i. Evaluate both models on the test set
  
  ii. Which metric did you choose and why?
  
  iii. Which model has better performance on the test set?
  
  iv. Compare the feature importance from the different models – do they agree? Are the top
       features similar in both models?
