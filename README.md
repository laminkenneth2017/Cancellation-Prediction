# Cancellation Prediction For Consumer Electronics
## PROJECT OUTLINE
1. Background
      - Business Problem
      - Project Primary Goal
      - Project Implication
2. Dataset Description
  Dataset Variables
      - Where has the data been gathered?
      - What are the input and output variables?
3. Description Analysis & Visualization 
        - Charts 
        - Chart insights
4. Data Preprocessing
    - Dropping columns and rows
    - Imputing missing values
    - Transforming variables
5. Fitting models and Classification
    - Logistic Regression Model, Decision Trees, Random Forests
    - Classification Report
6. Conclusion
    - Summary of Results
# Background  
## Business Problem(Background Statistics)
Consumers returned approximately $428 billion worth of goods in 2020, and this number continues to grow each year. In 2021, retail returns increased to an average of 16.6%, compared to 10.6% in 2020.
These statistics indicate that a high e-commerce cancellation rate is becoming the new norm, impacting profit margins, reducing retention rates, and hindering business scalability.
Firstly, canceled orders inflate operational costs without generating any return on investment. Additionally, customers who cancel orders often leave negative reviews, damaging business reputations and leading to customer churn.
Therefore, as an electronics retail stores that engages in e-commerce and aiming to scale the business, minimizing the cancellation rate is crucial. By doing so, the business can reduce churn, create positive impressions, and keep your customers returning.
### The Business Case: 
In the competitive electronic sales industry, understanding and improving order completion rates is critical for maximizing revenue and customer satisfaction. 
A high number of canceled orders can lead to lost sales, increased operational costs, and lower customer trust. 
However, manually tracking and analyzing every order to predict its completion likelihood is inefficient and impractical for large volumes of data. 
A data-driven approach that can automatically identify orders at risk of cancellation would allow the business to intervene proactively.

## Project Goal:
This project aims to develop a machine learning model to predict the completion status of orders based on transaction data. By accurately identifying the characteristics of completed versus canceled orders, the business can:
- [x] Improve Revenue: Focus on high-potential orders, minimizing the loss associated with cancellations.
- [x] Optimize Resource Allocation: Target promotional efforts towards customers and order types with a higher likelihood of completion.
- [x] Enhance Customer Experience: Reduce friction points that may lead to order cancellations, improving the overall customer journey.
### How will this goal be achieve:
This project aims to analyze electronic sales data from September 2023 to September 2024. Understanding sales patterns, customer behaviors, and product performance is crucial for the business. 

The goal is to improve sales strategies, optimize product offerings, and increase overall revenue.
### Implications: 
These insights can enhance marketing efforts, inventory management, and customer retention.

# Descriptive Analysis & Data Visualization 
The dataset consists of 20,000 records of electronic sales from September 2023 – September 2024, including product details, customer demographics, sales metrics, and transaction data.
### Variables/Data Types: 
Numerical 

Categorical 
- Total number of observations: 20,000
- Total number of variables: 16
## Descriptive Analytics 
- Numerical Variables
![image](https://github.com/user-attachments/assets/f0bf5cc2-dbc9-4d41-b234-10f5c78efa40)
-Correlation
![image](https://github.com/user-attachments/assets/b9191f54-babe-441a-beaf-50c10fd49f66)
The correlation statistics above describes the correlation between input variables(x) and the target variables. From the table above there is no true or high correlation between or among the input variables(x), but we can  see negative correlation between other variables which does not have any impact on the analysis.

## Data Visualization 
 - Correlation Matrix
![image](https://github.com/user-attachments/assets/a6c69e15-2fde-41ae-8619-12c6710bf758)

## Outliers 
![image](https://github.com/user-attachments/assets/3158ba46-ec37-4334-beea-09ac72af83cb)
The box plot on age and unit price has no outliers since there are no tiny dots located outside of the minimum or maximum whisker. However, the box plot on total sales has some outlier located above the maximum value.
## DATA VISUALIZATION con........
![image](https://github.com/user-attachments/assets/4a7fa574-a552-4d98-afd8-a18cc33ddbce)

![image](https://github.com/user-attachments/assets/e65186cb-1151-47f4-ba0f-f9ab073120d4)

![image](https://github.com/user-attachments/assets/f9fae3a6-9b43-4814-b460-ea17803ba1e2)

# Data Preprocessing
Dropping Variables, Encoding the Categorical Variables, Scaling, Combined the Processed, and Run Pipeline
![image](https://github.com/user-attachments/assets/088e5956-248e-48a5-80ce-2e56f5e1b2af)
Customer ID and SKU columns were dropped because they were not rlevant for the analysis.

# DATA MODELING
## Classification Models
Three different classification models were conducted:
- Random Forest  
- Logistic Regression 
- Decision Tree 
	- [x] Target variable  = Order Status
             1= Complete, 0= Cancelled
             
	- [x] Independent variables are: Age, Gender, Quantity, Total Sales, etc.
 The models were selected for their reliability and is common for classifying information
 
### Project Goal:
The goal is to develop a predictive model to identify factors influencing order completion, enabling better-targeted marketing strategies using machine learning models (logistic 	regression, decision tree, random forest), and provide actionable insights.









