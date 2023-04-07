# Home Loan Approval with Random Forest Classifier
## Introduction
The purpose of this project is to Classify customer loan applications as approved or denied. The data used in this project was sourced from Dream Housing Financing Company (DHFC) and found at https://www.kaggle.com/datasets/rishikeshkonapure/home-loan-approval. The dataset contains 614 entries. There are a total of 13 features (Loan_ID: The bank provided ID number for the loan request; Gender: String variable indicating Gender of the primary applicant; Married: String variable indicating marital status of primary applicant; Dependents: The number of dependents of the primary applicant; Education: String variable indicating whether primary applicant graduated or not; Self_Employed: String Variable indicating whether primary applicant is self employed or not; ApplicantIncome: The income of the primary applicant; CoapplicantIncome: The income of the co-applicant; LoanAmount: The amount (in thousands) the applicant wants to borrow; Loan_Amount_Term: The term (in months) in which the applicant will repay the loan; Credit_History: Binary variable representing whether applicant's credit history is good or bad; Property_Area: Categorical variable indcating the type of area the applicant is from; and Loan_Status: String variable indciating whether the loan was approved or denied). A Random Forest Classifier model was used for the classification of this data and classified the test data with an accuracy of 78%, and a F1-score of 56% for application denial and 85% for application apprival. Accordingly, this model solves the problem reasonably well.

![alt text](https://unsplash.com/photos/Ui4cy_D5oZ8)


## Business Understanding and Data Understanding

"The importance of a home loan classification model is significant for both borrowers and lenders.

For borrowers, a home loan approval model helps them understand their eligibility for a home loan and the amount they can borrow. It also enables them to plan their finances accordingly, including the repayment schedule and the interest rates.

For lenders, a home loan approval model helps them to assess the creditworthiness of the borrowers and determine the level of risk involved in lending to them. This model considers various factors such as the borrower's income, credit score, employment status, and other financial obligations.

In addition, a well-designed home loan approval model can improve the efficiency of the lending process by reducing the time and effort required to assess loan applications. This can lead to faster loan approvals and better customer satisfaction.

Overall, a home loan approval model plays a crucial role in enabling individuals to achieve their dream of homeownership and ensuring responsible lending practices by financial institutions." ChatGPT

## Modeling and Evaluation

Three models were tested in this project: 1) RandomForestClassifier using GridSearchCV, 2) RandomForestClassifier using RandomSearchCV, and 3)  Logistic Regression using RandomSearchCV.
Of the three models, RandomForestClassifier using GridSearchCV outperformed the other models by no more than two percentage points when measured by the metrics of accuracy, precision, recall, and F1-score. Although it was the model I selected, using Grid search is slow when compared to the other models, and the time it takes to run the model may not outwiegh its meager increases in accuracy , F1 score, and the other metrics for some users. However, once the hyperparameters are set it perfroms just as quickly as the other two models when predicting whether a loan should be appproved or denied.

## Conclusion

A home loan classification model that accurately classifies whether a loan applicant has been approved or not can have significant benefits for lenders. It can standardize the loan approval process, reduce the risk of loan defaults, save time for loan officers, help ensure compliance with regulatory requirements, and reduce of bias in the approval process.


## Repository Navigation

Link to Slide Deck
https://github.com/malmahdi/Home_Loan_Approval/blob/main/Home%20Loan%20Approval.pptx

Link to final notebook
https://github.com/malmahdi/Home_Loan_Approval/blob/main/index.ipynb

For reproduction of results copy the link of the index.ipynb file to a jupyter environment and run the model. 
