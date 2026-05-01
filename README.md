# Student Exam Performance Prediction

A machine learning web application that predicts a student’s math score based on demographic and academic inputs such as gender, race or ethnicity, parental level of education, lunch type, test preparation status, reading score, and writing score.

## Project Overview

This project demonstrates an end-to-end machine learning workflow, from data ingestion and preprocessing to model training, evaluation, and deployment with a Flask web interface. The application allows users to enter student details and receive a predicted math score instantly.

## Features

- Predicts student math performance using machine learning
- Interactive Flask-based web application
- Data preprocessing with missing value handling and encoding
- Model training and comparison across multiple regression algorithms
- Saves the best-performing model and preprocessing pipeline for inference
- Simple HTML form for real-time prediction

## Tech Stack

- Python
- Flask
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- CatBoost
- HTML

## Dataset

The project uses a student performance dataset containing features such as:

- Gender
- Race or ethnicity
- Parental level of education
- Lunch type
- Test preparation course
- Reading score
- Writing score
- Math score as the target variable

## Project Workflow

1. Data ingestion from the source dataset
2. Train-test split and storage of raw data in the artifacts folder
3. Data transformation using:
   - Missing value imputation
   - One-hot encoding for categorical features
   - Standard scaling for numerical features
4. Model training with multiple regression algorithms
5. Model evaluation using R2 score
6. Saving the best model and preprocessing object
7. Flask deployment for real-time prediction

## Models Used

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- K-Neighbors Regressor
- XGBRegressor
- CatBoost Regressor
- AdaBoost Regressor

## Web Application

The web app provides a form where users can enter student details and get a predicted math score. The app includes:

- Home page
- Prediction form
- Result display after prediction

## Project Structure

- `app.py`: Flask application entry point
- `src/components/`: data ingestion, transformation, and model training modules
- `src/pipeline/`: prediction pipeline
- `templates/`: HTML templates for the web interface
- `artifacts/`: saved datasets, preprocessing object, and trained model

## Installation

1. Clone the repository
2. Install dependencies from `requirements.txt`
3. Run the Flask app using `app.py`

## Usage

- Open the application in a browser
- Fill in the student details
- Click predict to get the estimated math score

## Results

The best model is selected based on validation performance and used for final prediction. The trained pipeline can estimate student math scores from new input data in real time.

## Future Improvements

- Add model monitoring
- Improve UI design
- Add more feature engineering
- Deploy the application to cloud platforms

## Author

Deepakaditya_13