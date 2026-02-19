# Student_performance_prediction

🎓 Student Performance Prediction
This project predicts a student’s exam score (continuous value) based on academic and lifestyle factors using LightGBM Regressor.
The goal of this project is to analyze how different factors such as study hours, sleep quality, attendance, and study method affect student performance.

🤖 Machine Learning Algorithm Used
✅ LightGBM Regressor

This project uses LightGBM (Light Gradient Boosting Machine) for regression.

LightGBM is a powerful gradient boosting algorithm designed for:

Complex structured datasets

Non-linear relationships

High performance and fast training

🧠 Why LightGBM?

The dataset contains:

Mixed data types (numerical + categorical)

Complex feature interactions

Non-linear relationships between inputs and exam score

LightGBM is better than Linear Regression because:

It captures complex patterns

It handles feature interactions automatically

It provides better prediction accuracy

It reduces overfitting using boosting
Built using:

🐍 Python

📊 Pandas

🤖 Scikit-learn

🎛 Gradio

🚀 Hugging Face Spaces

📌 Project Overview

The model considers 11 input features such as:

Age

Gender

Course

Study Hours

Class Attendance

Internet Access

Sleep Hours

Sleep Quality

Study Method

Facility Rating

Exam Difficulty

📂 Dataset Information
Target Variable:
exam_score (float)

Features Used for Training:
age
gender
course
study_hours
class_attendance
internet_access
sleep_hours
sleep_quality
study_method
facility_rating
exam_difficulty


Note:

id column was removed during training.

Categorical features were encoded using pd.get_dummies().

⚙️ Model Training

Steps followed:

Load dataset

Drop unnecessary column (id)

Separate features and target

Apply One-Hot Encoding (pd.get_dummies)

Train regression model

Save model using joblib

🖥 Web Application (Gradio)

The app allows users to enter student details and get a predicted exam score instantly.

Important:

Since the model was trained on encoded features, the app:

Applies pd.get_dummies() on input

Aligns columns with model.feature_names_in_

Fills missing columns with 0

This ensures no column mismatch errors.

▶️ How to Run Locally
pip install -r requirements.txt
python app.py


App will run on:

http://localhost:7860

📦 Project Structure
├── app.py
├── student_perfomance_model.pkl
├── train.csv
├── test.csv
├── README.md

🚀 Deployment

This project can be deployed on:

Hugging Face Spaces

Render

Railway

Streamlit Cloud

🧠 Future Improvements

Use Pipeline instead of manual encoding

Add input validation

Improve UI design

Add performance metrics display

👩‍💻 Author
Jagruti Dhangar
deployed link:https://jagruti512-student-perfomace-project.hf.space/?logs=container&__theme=system&deep_link=ejht-MVUCN8

✅ requirements.txt file

