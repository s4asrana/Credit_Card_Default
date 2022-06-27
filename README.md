# Credit_Card_Default using SVM

The task here is to classify whether a person will default or not on their credit card using various feautures like age, sex, marital status, past payments etc.

To accomplish the task I built support vector machine for classification(using scikit learn and the Radial Basis Function(RBF) kernel). The training dataset contains both continuous and categorical data from the UCI Machine Learning Repository to classify whether a person will default or not on their credit card.

For this problem I used the following steps:   

1. Importing the data and necessary libraries.
2. Identifying and handling missing values. 
3. Downsampling data. 
4. Train-test split the data.
5. Building a preliminary svm.
6. Doing hyperparamter tuning to find the best optimization parameters like gamma.
7. Evaluating and interpreting the final svm.

    
Data Description:

The training dataset contains both continuous and categorical data from the UCI Machine Learning Repository to classify whether a person wil default or not on their credit card.
    
    **ID** The ID number of each customer.                                                                              
    **LIMIT_BAL** Credit Limit(it includes both the individual consumer credit and his/her family (supplementary) credit.)                                                                                               
    **SEX** Gender((1 = male; 2 = female)                                                                               
    **EDUCATION** (1 = graduate school; 2 = university; 3 = high school; 4 = others).                                   
    **Marital status** (1 = married; 2 = single; 3 = others).                                                          
    **Age** in year.                                                                                                     
    **PAY_X** History of past payment(When the last 6 bills were payed)
            -1 = pay duly; 1 = payment delay for one month; 2 = payment delay for two months; . . .; 8 = payment delay for eight months; 9 = payment delay for nine months and above.                                             
    **BILL_AMTX** What the last 6 bills were.                                                                           
    **PAY_AMTX** How much the last payments were.                                                                       
    **default payment next month** Whether a defaulter or not(1=yes, 0=no)
