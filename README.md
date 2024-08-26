# Employee Churn Prediction
## Project Overview
This project aims to predict employee churn by identifying key factors that influence their decision to leave the company. By leveraging historical data and machine learning techniques, the project helps in identifying at-risk employees and provides actionable insights for improving employee retention.
## Key Tools and Technologies
- Google Cloud Platform (GCP): This is used for data storage, querying, and management using BigQuery.
- Google Colab: This is for data analysis and model training. (Python & PyCaret - For machine learning model development and automation.)
- Looker Studio: For building an interactive and insightful dashboard.
## Data Overview
- **tbl_hr_data:** Contains 15,004 rows of historical employee data.
- **tbl_new_employees:** Contains 100 rows of new employee data for model testing.
These datasets were combined and processed in BigQuery to create a unified view, facilitating efficient model training and analysis.
## Project Workflow
1. **Data Ingestion (BigQuery):** Load historical employee data and new employee data into BigQuery.
2. **Data Processing (Google Colab):** Connect to BigQuery from Google Colab. Combine datasets, perform data cleaning, and apply transformations using Python in Google Colab.
3. **Model Development (Google Colab):** Build and train the churn prediction model using PyCaret in Python.
4. **Model Evaluation (Google Colab & BigQuery):** Test and validate the model in Google Colab. Return the predictions and feature importance scores back to BigQuery.
5. **Data Visualization (Looker Studio):** Connect BigQuery to Looker Studio. Create a dashboard to visualize insights, predictions, and key factors contributing to employee churn.

## Modeling Approach
The predictive model was developed using PyCaret, an open-source, low-code machine learning library in Python, which simplifies the process of building and deploying machine learning models. The modeling workflow included the following steps:

- **Data Connection:** The Colab notebook was connected to BigQuery to retrieve and manipulate the necessary data.
- **Model Training:** The model, primarily using the Random Forest algorithm, was trained on historical data to identify patterns related to employee churn.
- **Prediction and Evaluation:** The model's performance was evaluated, and predictions were made on new employee data to assess churn risk.
- **Feature Importance:** The analysis highlighted job satisfaction as the most significant predictor of employee churn, alongside other influential factors.

## Dashboard and Insights [(Link)]([https://lookerstudio.google.com/embed/reporting/726ff6ed-2e85-4ef2-b602-74e5d96e4ba7/page/Y9s9D])
An interactive dashboard was developed using Looker Studio to visualize the model's predictions and feature importance. The dashboard provides a comprehensive overview of employee churn trends, satisfaction levels, and departmental churn rates. These insights empower stakeholders to make informed, data-driven decisions to mitigate churn and improve employee retention.

