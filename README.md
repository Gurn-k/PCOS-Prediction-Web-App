# 👩‍⚕️ PCOS Prediction Web Application (Flask + Scikit-learn)

This project is a machine learning-based web application built with Python and the Flask framework. It is designed to predict the likelihood of Polycystic Ovary Syndrome (PCOS) based on various clinical and metabolic input parameters submitted through a user-friendly web form.

# 🎯 Key Features

Model: Random Forest Classifier achieving approximately 92% accuracy on the training dataset.

Technology: Python, Flask (Web Framework), Pandas, Scikit-learn (Machine Learning).

Web Interface: Allows real-time interaction and prediction via a local web browser.

# ⚙️ Setup and Installation

IMPORTANT: Due to version conflicts with the original project, the model must be retrained locally using the latest compatible libraries. Follow these steps precisely.

1. Clone the Repository

git clone [https://github.com/Gurn-k/PCOS-Prediction-Web-App.git](https://github.com/Gurn-k/PCOS-Prediction-Web-App.git)
cd PCOS-Prediction-Web-App


2. Create and Activate Virtual Environment

A virtual environment (venv) is necessary to manage project dependencies.

For Windows (PowerShell/CMD):

python -m venv venv
.\venv\Scripts\activate


(Your terminal prompt must show (venv))

3. Install All Dependencies

Install all necessary libraries (Flask, Scikit-learn, Pandas, Matplotlib, and Seaborn):

pip install flask scikit-learn pandas numpy matplotlib seaborn


# ▶️ How to Run the Application

Step 1: Retrain the Model

Run the training script to generate a new model.pkl file compatible with your installed library versions:

python model.py


(A successful run will display the model's accuracy.)

Step 2: Start the Web Server

Launch the Flask application:

python app.py


Step 3: Access the App

Open your web browser and navigate to the local address provided in the terminal:

http://127.0.0.1:5000/

# 📂 Project Structure

File/Folder

Description

app.py

The main Flask application that loads the model and handles web requests.

model.py

The data processing and model training script.

model.pkl

The trained Random Forest model file.

PCOS_data.csv

The dataset used for training the model.

templates/

Directory containing the application's HTML templates.
