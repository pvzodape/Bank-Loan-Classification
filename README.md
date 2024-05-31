# Bank-Loan-Classification
A classification model to simplify the loan approval processes for banks.
### Overview
**Introduction:** A loan is a major source of income for banks while lending banks undergo a necessary verification process by evaluating the client, their demographics, credit history, and loan amount to decide whether or not to approve the loan.

Identifying whether to approve a loan can be solved using ML in modern times using classification.

**Data Source:** This data is downloaded from Kaggle. The data set used has 13 columns and 615 rows.

**Columns:** 
1. **Loan_ID**: Unique Id Assigned to customers, object data type, independent variable
2. **Gender**: Male, Female, object data type, independent variable 
3. **Married**: Marital status, object data type, independent variable 
4. **Dependents**: Number of dependent count, object data type, independent variable 
5. **Education**: Graduate, Not Graduate, object data type, independent variable 
6. **Self_Employed**: Yes, No, object data type, independent variable 
7. **applicantincome**: Income, Int data type, independent variable 
8. **Coapplicantincome**: co-applicant income, int datatype, independent variable 
9. **LoanaAmount**: Loan amount, int data type, independent variable 
10. **Loan_Amount_Term**: Days for which loan is taken, int data type, independent variable 
11. **Credit_History**: 1 indicates credit paid, 0 indicates loan not paid previously, int data type, independent variable 
12. **Property_Area**: Area in which the property is located namely urban or rural, independent variable 
13. **Loan_Status**: Loan is approved or not 'Y'= Approved, 'N' = Not Approved, dependent Variable

### Steps Involved: 
1. **Filling Null Values:** Filled numeric data using median since outliers were present, columns with object data types were filled with mode.
2. **Feature Engineering:** Created new column by combining applicantincome and Coapplicantincome, normalized the data
3. **Model_Training:** Trained the model, checked accuracy score, and classified using logistic regression, decision tree, random forest, and k neighbor classifier.
4. **Analysis Report** Compared the result of these classifiers and the data was found overfitted.
5. **Balancing Data Set:** Balanced the data set
6. **Revaluated the model:** Revaluated the model with balanced data.

The accuracy score of the Random Forest Classifier was found to be highest 88%
   
