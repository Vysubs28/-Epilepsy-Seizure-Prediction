# 🧠 Epileptic Seizure Detection from EEG Data

This project uses a machine learning model to classify EEG (electroencephalogram) data and detect signs of epileptic seizures. Built using scikit-learn, pandas, and deployed as an interactive app via Gradio on Hugging Face Spaces.

## 🚀 Live Demo

👉 [Try the app on Hugging Face Spaces](https://huggingface.co/spaces/vysubs28/epilepsy-predictor) 
*(Replace the link with your actual Space URL)*

## 📈 Model Performance

| Metric       | Score  |
|--------------|--------|
| Accuracy     | 91.03% |
| Precision (0)| 45%    |
| Recall (0)   | 26%    |
| Precision (1)| 93%    |
| Recall (1)   | 97%    |
| F1-score (1) | 95%    |

> Class `1` represents seizure activity; class `0` represents non-seizure.

---

## 🗂️ Project Structure

├── app.py # Gradio web app
├── eeg_data.csv # EEG dataset (sample or full)
├── model.joblib # Trained classification model
├── requirements.txt # Python dependencies
├── Epilepsy_.ipynb # Notebook used to train and evaluate the model
└── README.md # You're here!

yaml
Copy
Edit

---

## 📦 Installation & Local Development

Clone the repo and install dependencies:

```bash
git clone https://github.com/your-username/epilepsy-detection-app.git
cd epilepsy-detection-app
pip install -r requirements.txt
python app.py
The app will open in your browser via Gradio.

💡 How It Works
EEG data is preprocessed and fed into a trained machine learning model.

The model classifies the data into seizure (1) or non-seizure (0).

The Gradio interface allows users to input new data and get real-time predictions.
🧪 Test Input Example
To help you get started, here’s an example of realistic EEG feature values that will trigger a seizure (epileptic) prediction:

Feature	Example Value
feature_0 (FP1 δ)	125.4
feature_1 (FP1 θ)	98.7
feature_2 (FP1 α)	87.6
feature_3 (FP1 β)	45.3
feature_4 (FP1 γ)	23.9
feature_5 (FP2 δ)	112.1
feature_6 (FP2 θ)	90.5
feature_7 (FP2 α)	80.2
feature_8 (FP2 β)	50.7

🔎 These values simulate typical EEG readings with elevated brainwave activity consistent with seizure conditions.
You can copy and paste these directly into the live app on Hugging Face.

🧠 Tip for Users
If you're unsure what values to try:

Use float values (e.g., 85.3, not just 85).

Don't input all 0s — that's not a valid EEG signal.

Try adjusting values one at a time to see how predictions change.


📚 Dependencies
scikit-learn

numpy

pandas

gradio

joblib

matplotlib

transformers

torch

All dependencies are listed in requirements.txt.

📄 License
MIT License

🙌 Acknowledgments
Thanks to the open-source community and researchers providing EEG datasets for enabling accessible seizure detection research.
