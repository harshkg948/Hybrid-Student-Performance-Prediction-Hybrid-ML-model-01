# Hybrid-Student-Performance-Prediction-Hybrid-ML-model-01
Hybrid ML model by using unsupervised and supervised ml
📊 Student Performance Prediction using Hybrid ML
🚀 Overview

This project explores a hybrid machine learning approach combining both unsupervised learning (clustering) and supervised learning (logistic regression) to analyze and predict student performance.

The main idea is to:

Derive meaningful patterns from student scores
Automatically generate performance categories using clustering
Use those categories as labels for a predictive model
📁 Dataset
Student Performance Dataset (CSV)
Features include:
Math Score
Reading Score
Writing Score
Test Preparation Course
🧠 Methodology
1. 📌 Data Preprocessing

Calculated average score:

average_score = (math + reading + writing) / 3
Encoded categorical feature:
test preparation course → numerical using Label Encoding
2. 🔍 Unsupervised Learning (Clustering)
Applied clustering algorithm (e.g., K-Means)
Input feature:
average_score
Output:
Generated clusters representing performance groups
Converted clusters into:
grade_enco (encoded grade labels)
3. 🤖 Supervised Learning (Logistic Regression)
Model: Logistic Regression
Input Features:
average_score
test_preparation_encoded
Target:
grade_enco
4. 📈 Model Evaluation
Metric used:
Recall Score = 1.0
f1 score = 1.0
This indicates that the model successfully identified all instances of the target class in the evaluation dataset.

⚙️ Tech Stack
Python 🐍
Pandas
NumPy
Scikit-learn
🔄 Workflow Pipeline
Load Dataset
Data Cleaning & Feature Engineering
Compute Average Score
Encode Categorical Features
Apply Clustering → Generate Labels
Train Logistic Regression Model
Evaluate Performance
💡 Key Insights
Clustering helps in automatically discovering performance groups
Combining unsupervised + supervised learning creates a hybrid ML pipeline
Feature engineering (average score) plays a crucial role in model performance
⚠️ Note

This project is implemented on a small dataset for learning purposes.
The clustering-based labels are derived from input features, which may lead to very high evaluation scores.

🚀 Future Improvements
Use larger and more complex datasets
Introduce additional features (study time, attendance, etc.)
Replace average score with raw subject scores
Try advanced models (Random Forest, XGBoost)
Deploy using Flask / Streamlit
📌 Author

Harsh Gupta
