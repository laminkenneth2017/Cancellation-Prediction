### CLIKE HERE TO DOWNLOAD PYTHON/PYSPARK CODE: [Term_Project.ipynb.pdf](https://github.com/user-attachments/files/18992686/Term_Project.ipynb.pdf)

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
The goal is to develop a predictive model to identify factors influencing order completion, enabling better-targeted marketing strategies using machine learning models (logistic regression, decision tree, random forest), and provide actionable insights. By accurately identifying the characteristics of completed versus canceled orders, the business can:

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

## Making Prediction and Model Assessment
![image](https://github.com/user-attachments/assets/2370e3a8-0652-4158-9ccc-c9ac8061b4de)

### Logistic Regression:
has the highest accuracy (0.67477) and recall (0.6747701), suggesting it performs well in overall correct predictions and identifying actual "Completed" orders. However, its AUC (0.494772) is the lowest, indicating weaker class distinction.

### Decision Tree:
Has the highest precision (0.6482259) and the best AUC (0.504184), meaning it minimizes false positives and is better at distinguishing between "Completed" and "Canceled" orders. Its accuracy (0.6695639) and recall (0.669563) are only slightly lower than Logistic Regression, showing a balanced performance.

### Random Forest:
Has similar accuracy and recall to Decision Tree but the lowest precision (0.44650502) and F-measure (0.535310233), indicating it has more false positives when predicting "Completed" orders.

- [x] The Decision Tree model is the best choice for this project due to its high precision, best AUC, and balanced performance, making it more reliable for distinguishing between completed and canceled orders.

# ROC Curve AUC - AUC :0.50
![image](https://github.com/user-attachments/assets/59bb074b-5995-4dfe-8d82-2dbbdf6c5fd0)

# INSIGHT - CONCLUSION

## Key Insights

### Best Model: 

The Decision Tree model outperformed the others, achieving the highest precision and AUC. This model provides a balanced performance in identifying completed orders with fewer false positives, making it the most suitable for this classification task.

### Feature Impact: 

Variables such as Total Sales and Quantity showed significant influence on the likelihood of order completion, and highlighting potential areas for business improvement. For instance, orders with higher quantities may have a higher probability of being completed.

### Business Implications: 

By accurately predicting order status, the business can target resources more effectively, improve customer satisfaction, and reduce cancellations. Insights from the model can inform strategies to enhance customer retention and optimize marketing efforts for likely completed orders.

## Conclusion

The project demonstrates that predictive modeling, particularly using Decision Trees, can provide valuable insights into factors affecting order outcomes. By implementing this model, the business can make data-driven decisions to enhance sales efficiency and customer loyalty. Future analysis can explore additional features and more advanced models to further improve prediction accuracy.



Sources: https://blog.fabrichq.ai/what-is-order-cancellation-in-ecommerce-and-how-can-you-reduce-it-6076f8e6a0d5

Data source: https://www.kaggle.com/datasets/cameronseamons/electronic-sales-sep2023-sep2024






