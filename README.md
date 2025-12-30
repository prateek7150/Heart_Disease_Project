# ❤️ Heart Disease Prediction (Machine Learning + Streamlit)

## 📌 Overview
This project predicts the chances of **heart disease** using machine learning.  
It provides an interactive **Streamlit web application** where users can input clinical parameters and receive a risk prediction.

## 🧠 Model Benchmarking
Several machine learning algorithms were tested on the dataset (`heart.csv`) to identify the best-performing model:

- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- Naive Bayes  
- Decision Tree  
- Support Vector Machine (SVM)  

After calculating **Accuracy** and **F1 Score** for each model, **SVM was finalized** as the most reliable algorithm.

| Model               | Accuracy | F1 Score |
|----------------------|----------|----------|
| Logistic Regression  | 0.8779   | 0.894    |
| KNN                  | 0.8581   | 0.8732   |
| Naive Bayes          | 0.8713   | 0.8876   |
| Decision Tree        | 0.7657   | 0.7893   |
| **SVM (Final)**      | **0.8812** | **0.8977** |

## ⚙️ Features in the App
The app collects the following parameters from the user:
- Age  
- Sex  
- Chest Pain Type  
- Resting Blood Pressure  
- Cholesterol  
- Fasting Blood Sugar  
- Resting ECG  
- Max Heart Rate  
- Exercise-Induced Angina  
- Oldpeak (ST Depression)  
- ST Slope  

These inputs are preprocessed using a **scaler** and matched against the **expected feature columns** before prediction.

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/prateek7150/Heart_Disease_Project.git
   cd Heart_Disease_Project
2.Install Dependencies

  pip install -r requirements.txt


3.Run The Streamlit App
  streamlit run app.py



Project Structure

Heart_Disease_Project/
│-- app.py              # Streamlit UI
│-- heart.csv           # Dataset
│-- Heart_disease.ipynb # Model training notebook
│-- SVM_heart.pkl       # Final trained SVM model
│-- scaler.pkl          # Scaler for preprocessing
│-- columns.pkl         # Expected feature columns
│-- requirements.txt    # Dependencies
│-- .gitignore
  
   
