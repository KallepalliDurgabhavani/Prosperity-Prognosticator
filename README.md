# Prosperity Prognosticator  
Machine Learning for Startup Success Prediction

A Flask-based web application that predicts whether a startup will be Acquired or Closed using a Random Forest classifier trained on real startup data.

---

## Project Overview

Prosperity Prognosticator helps investors, entrepreneurs, and policymakers analyze startup success probability by entering key funding and milestone metrics.

Team ID: LTVIP2026TMIDS76348  
Project Name: Prosperity Prognosticator  
Date: 30 January 2026  
Algorithm: Random Forest Classifier  
Dataset: startup1.csv (923 startups)  
Model Accuracy: 83.82%

---

## Project Structure

Project Executable Files/

app.py – Flask web server  
random_forest_model.pkl – Trained Random Forest model  
startup1.csv – Dataset used for training  
Startup_Success_Prediction.ipynb – Model training and analysis notebook  

template/  
index.html – Home page  
result.html – Prediction result page  

---

## Tech Stack

Python 3.8+ – Core programming  
Flask – Web framework  
Scikit-learn – Machine learning model  
Pandas & NumPy – Data processing  
Joblib – Model saving/loading  
HTML5 & CSS3 – Frontend UI  

---

## Input Features

1. age_first_funding_year – Years after founding when first funding was received  
2. age_last_funding_year – Years after founding when last funding was received  
3. age_first_milestone_year – Years after founding when first milestone was achieved  
4. age_last_milestone_year – Years after founding when last milestone was achieved  
5. relationships – Number of business relationships  
6. funding_rounds – Number of funding rounds  
7. funding_total_usd – Total funding in USD  
8. milestones – Total milestones achieved  
9. avg_participants – Average investors per funding round  

---

## Model Performance

Training Accuracy: 100%  
Testing Accuracy: 83.82%  
Precision: 0.84  
Recall: 0.83  
F1-Score: 0.84  
ROC-AUC: 0.91  

---

## How to Run the Project

Step 1: Open Anaconda Prompt and go to project folder

cd "C:\Users\YourName\Project Executable Files"

Step 2: Install required packages

pip install flask joblib numpy pandas scikit-learn

Step 3: Run the Flask app

python app.py

Step 4: Open browser and go to

http://127.0.0.1:5000

---

## Application Routes

/       GET   Home page (index.html)  
/predict GET/POST Receives input and predicts result  
/result  Displays prediction result  

---

## How It Works

1. User opens the home page  
2. User enters startup metrics  
3. Flask receives data via /predict  
4. Model predicts Acquired (1) or Closed (0)  
5. Result page shows prediction  

---

## Troubleshooting

ModuleNotFoundError: flask  
Run: pip install flask  

FileNotFoundError: random_forest_model.pkl  
Ensure .pkl file is in the same folder as app.py  

TemplateNotFound: index.html  
Ensure folder name is exactly "template"  

Port 5000 already in use  
Change port in app.py to app.run(port=5001)  

---

## Team Details

Team ID: LTVIP2026TMIDS76348  
Project Phase: Project Development Phase  
Date: 30 January 2026  

---

## Built With

Python, Flask, Scikit-learn, Pandas, NumPy, HTML, CSS
