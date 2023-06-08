# Project-Four
## Team Members: 
Brittany Wright, Jorge Chavez, Karen Fuentes, Alejandra Gomez

## Project Requirements
For Project 4, you will work with your group to solve, analyze, or visualize a problem using machine learning (ML) with the other technologies we’ve learned. Here are the specific requirements:

1. Find a problem worth solving, analyzing, or visualizing.
2. Use machine learning (ML) with the technologies we’ve learned.
3. You must use Scikit-learn and/or another machine learning library.
4. Your project must be powered by a dataset with at least 100 records.
5. You must use at least two of the following:
    - Python Pandas **
    - Python Matplotlib **
    - HTML/CSS/Bootstrap
    - JavaScript Plotly
    - JavaScript Leaflet
    - SQL Database
    - MongoDB Database
    - Google Cloud SQL
    - Amazon AWS **
    - Tableau **

** Used in project

## Project Proposal
The aim of our project is to uncover patterns between loan information and loan applicant information. We will attempt to predict loan status based on credit scores as well as examine relationships between income and credit score. We will also look at other related relationships between age, credit score, loan amount and loan status.

The questions/predictions we will ask of the data:
   1. Predicting loan status based on credit scores?
   2. Relationship between income to credit score?
   3. Relationship between age, credit score, loan amount and status.

Data Source: https://www.kaggle.com/datasets/ychope/loan-approval-dataset

Data Preview

![image](https://github.com/agomezsaenz05/Project-Four/assets/120424668/ce4a5206-3f97-4f49-a12a-bbf235ecb563)

## Data Cleaning
- Merged the training and testing datasets from Kaggle (full_loan_dataset.csv)
- Dropped all null values
- Dropped outlier credit scores
- Recoded the “Loan Status” variable

** datasets are located in "Data" folder **

## Data Visualizations
- Imported our merged dataset into Tableau
- Created visualizations with different variables to help us see relationships between the data
- Tableau Public Link: https://public.tableau.com/views/Project-Four_Group-3/CreditScoreSummary?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link
- Tableau file: Project-Four_Group-3.twbx

## Data Model Implementation & Optimization
### Random Forest
- We used the top 10 most important features
- Accuracy Score: 0.84
- Classifying Fully Paid
	- Precision: 0.84
	- Recall: 1.00
- Classifying Charged Off
	- Precision: 0.63
	- Recall: 0.01
### Logistic Regression
- Decided to use top 9 from random forest originally since the last feature only explained roughly 1% of the variance.
- Accuracy: 0.84
- Classifying Fully Paid
	- Precision: 0.84
	- Recall: 1.00
- Classifying Charged Off
	- Precision: 0.00
	- Recall: 0.00
### Changing the number of predictors
- Changed the number of predictors to the top 5 as each explained roughly 10% of the variance.
- Predictors included current loan amount, monthly debt, maximum open credit, current credit balance. 




******************************* DELETE BEFORE SUBMITTING **************************************	
## Requirements
Data Model Implementation (25 points)

- A Python script initializes, trains, and evaluates a model (10 points)
- The data is cleaned, normalized, and standardized prior to modeling (5 points)
- The model utilizes data retrieved from SQL or Spark (5 points)
- The model demonstrates meaningful predictive power at least 75% classification accuracy or 0.80 R-squared. (5 points)

Data Model Optimization (25 points)
- The model optimization and evaluation process showing iterative changes made to the model and the resulting changes in model performance is documented in either a CSV/Excel table or in the Python script itself (15 points)
- Overall model performance is printed or displayed at the end of the script (10 points)

GitHub Documentation (25 points)
- GitHub repository is free of unnecessary files and folders and has an appropriate .gitignore in use (10 points)
- The README is customized as a polished presentation of the content of the project (15 points)

Group Presentation (25 points)
- All group members speak during the presentation. (5 points)
- Content, transitions, and conclusions flow smoothly within any time restrictions. (5 points)
- The content is relevant to the project. (10 points)
- The presentation maintains audience interest. (5 points)
