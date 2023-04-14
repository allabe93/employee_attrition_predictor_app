![Alt text for the image](https://raw.githubusercontent.com/allabe93/employee_attrition_predictor/main/quitting.jpg)

# employee_attrition_predictor

This project aims to predict employee attrition based on various features such as age, salary, job satisfaction, work-life balance, years at the company, and others. The main objective is to help organizations identify potential employee attrition risks and take appropriate actions to retain valuable employees.

To achieve this goal we created a Streamlit web app which predicts the probability of employee attrition using a logistic regression model that was trained on preprocessed data. The app starts by importing necessary libraries and loading the files (data, scaler, and model) and sets up the structure of the web page with headers, an image, and text. It then generates input fields for each feature using the generate_input() function and the st.selectbox() function for the overtime feature. The user inputs are collected and preprocessed (e.g., encoding the overtime feature and scaling the input data) before being fed into the saved logistic regression model to generate a prediction. The prediction is then displayed as a probability, with different colors depending on the risk level of employee attrition.
The "magic" happens when the user's input data is gathered, preprocessed, and the trained model is used to make a prediction. Once the prediction is achieved, it can be displayed it to the user with appropriate formatting

## Overview
The project consists of several components:
1.	Data Analysis and Feature Engineering: exploratory data analysis was performed on the IBM HR Analytics Employee Attrition & Performance dataset from Kaggle, and features were engineered for better model performance.
2.	Machine Learning Model: Logistic Regression was chosen as the best performing model in terms of recall for the minority class (attrition). SMOTE was used to balance the dataset, and hyperparameter tuning was applied to improve the model further.
3.	Web Application: a Streamlit web application was developed to provide an interactive user interface for inputting employee data and predicting the probability of attrition.

## Project Structure
•	data/: Contains the dataset used for the project.
•	pickle_files/: Contains the saved scaler and Logistic Regression model files.
•	app.py: The Streamlit web application.
•	Employee_Attrition_Predictor.ipynb: The Jupyter Notebook containing the data analysis, feature engineering, and machine learning model development process.

## Key Findings
1.	Logistic Regression was chosen as the best model due to its high recall for the minority class (attrition), which is important for this project's objective of predicting employee attrition.
2.	The use of SMOTE (oversampling technique) and hyperparameter tuning resulted in improved model performance.
3.	Several features, such as monthly income, job satisfaction, and work-life balance, were found to have significant influence on employee attrition.

## Libraries Used
•	Numpy: https://numpy.org/doc/stable/

•	Pandas: https://pandas.pydata.org/pandas-docs/stable/index.html

•	Seaborn: https://seaborn.pydata.org/

•	Matplotlib: https://matplotlib.org/stable/contents.html

•	Scikit-learn: https://scikit-learn.org/stable/user_guide.html

•	Imbalanced-learn: https://imbalanced-learn.org/stable/

•	Streamlit: https://docs.streamlit.io/en/stable/
