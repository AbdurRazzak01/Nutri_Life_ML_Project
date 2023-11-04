# Nutri_Life_ML_Project


Description:
This project aims to create a Nutri-Score calculator for food products available in the United Kingdom. Nutri-Score is a nutrition label that provides at-a-glance information about the nutritional quality of a food product. The purpose of this project is to help consumers make healthier food choices by categorizing products and calculating their Nutri-Score based on various nutritional attributes. By leveraging machine learning techniques, this tool offers an interactive interface for users to search and evaluate different food products, promoting informed dietary decisions.

Introduction:
In today's fast-paced world, making healthy food choices is crucial for maintaining overall well-being. However, understanding the nutritional content of various food products can be challenging for consumers. The Nutri-Score calculator project addresses this challenge by providing an intuitive platform for users in the UK to assess the nutritional quality of food items effortlessly. By categorizing products and calculating Nutri-Score based on key nutritional factors, this project empowers individuals to make informed decisions about their diet, promoting healthier lifestyles and contributing to improved public health.

Technologies Used:
Python: The project is implemented using the Python programming language.
Pandas: Pandas is used for data manipulation and analysis, facilitating the handling of the dataset.
scikit-learn: The scikit-learn library is utilized for machine learning tasks, including imputation and regression modeling.
HistGradientBoostingRegressor: This regressor from scikit-learn is employed for model-based imputation of missing values in the dataset.
LabelEncoder: LabelEncoder from scikit-learn is used to encode categorical variables into numerical format.
openpyxl: The openpyxl engine is utilized to read Excel files, enabling seamless data ingestion.
This project showcases the intersection of data science and nutrition, offering a practical solution to enhance public awareness about the nutritional content of food products. Through the application of machine learning algorithms and interactive user interfaces, it bridges the gap between complex nutritional data and everyday consumers, encouraging healthier dietary choices in the United Kingdom.

Project Structure:
The project directory is organized as follows:

/data: Contains the dataset files, including Final_UK_Food_Product.xlsx, which stores the raw data.
/src: This directory houses the Python source code files.
data_preparation.py: Handles data sourcing, preprocessing, missing value imputation, and feature engineering.
nutri_score_calculator.py: Implements the Nutri-Score calculation logic.
user_interaction.py: Manages user input processing and interaction.
/output: Stores the output files or processed datasets.
README.md: Provides project documentation and instructions for users and developers.

Data Preparation:
Data Sourcing:
The dataset, Final_UK_Food_Product.xlsx, was sourced from a reliable nutrition database, providing detailed information about various food products available in the United Kingdom.

Data Preprocessing Steps:

Filtering Data: Rows containing products from the United Kingdom were filtered using the 'countries_en' column.
Label Encoding: Non-numeric columns such as 'main_category' were label-encoded for model input.
Handling Missing Values: Missing values in selected nutritional columns were imputed using the HistGradientBoostingRegressor model. Data was split into features and target variables for training and prediction.
Feature Engineering: The 'nutri_score' was calculated based on a weighted combination of nutritional attributes, representing the overall nutritional quality of each product.

Machine Learning Model:
Algorithm:
The project employed the HistGradientBoostingRegressor algorithm from the scikit-learn library for model-based imputation of missing values. This algorithm is robust, handles large datasets efficiently, and provides accurate predictions.

Hyperparameter Tuning:
The model's hyperparameters were set to default values for simplicity in this project. However, for a real-world application, hyperparameters could be fine-tuned using techniques like grid search or randomized search to optimize the model's performance.

User Interaction:
User Input Processing:
The user can input a product name or category of interest.

Example 1: User inputs 'chocolate'. The system searches and displays chocolate products and their Nutri-Score ratings.
Example 2: User inputs 'snacks'. The system filters snacks products and presents their Nutri-Score information.
Expected Outcomes:

The system returns a list of products matching the user's input, along with their respective Nutri-Score ratings.
Users can make informed decisions based on the Nutri-Score and product categories, promoting healthier food choices.
This interactive feature enhances user engagement, making it easier for consumers to access nutritional information and choose healthier food options.





