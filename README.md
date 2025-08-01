# -Epilepsy-Seizure-Prediction
This project uses a machine learning model to detect epileptic seizures from EEG (electroencephalogram) data. The app is deployed on Hugging Face Spaces with a simple Gradio interface for real-time inference.
🚀 Live Demo
👉 Try the app on Hugging Face Spaces

📁 Project Contents
app.py – The Gradio app for running inference

eeg_data.csv – EEG data used for processing or display

model.joblib – Trained machine learning model

requirements.txt – Python dependencies

Epilepsy_.ipynb – Original training and evaluation notebook

README.md – Project description and usage

📊 Model Performance
Accuracy: 91%

Precision (Class 1): 93%

Recall (Class 1): 97%

🧪 How to Run Locally
bash
Copy
Edit
git clone https://github.com/your-username/your-repo.git
cd your-repo
pip install -r requirements.txt
python app.py
