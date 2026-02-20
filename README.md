# HDFC-BANK-RETAIL-CREDIT-CARD-CHURN-PREDICTION
A machine learning–powered web application to predict credit card customer churn for HDFC Bank retail clients using demographic, behavioral, and financial attributes.
Built with Python, Scikit-learn, and Streamlit, and deployed as an interactive prediction system.

📌 Problem Statement

Customer churn is a major challenge for retail banks. Losing an existing credit card customer is far more expensive than retaining one.

This project predicts whether a customer is likely to churn (leave the bank) based on historical customer data, enabling proactive retention strategies.

🚀 Features

Interactive Streamlit web application

End-to-end ML pipeline (preprocessing + model)

Handles categorical & numerical features

Real-time churn prediction

Clean UI with structured inputs

Serialized artifacts for reproducibility

🧠 Machine Learning Pipeline

Data Preprocessing

Encoding categorical variables

Feature scaling

Model Training

Supervised classification model

Inference

Single-customer prediction

Strict feature schema enforcement

Artifacts used:

transformer_hdfc_churn_pipeline.pkl – preprocessing + model pipeline

target_encoder.pkl – label encoder

Hdfc bank model.pkl – trained model

🛠️ Tech Stack

Python 3

Pandas, NumPy

Scikit-learn

Joblib

Streamlit

📂 Project Structure
HDFC-BANK-RETAIL-CREDIT-CARD-CHURN-PREDICTION/
│
├── app.py                          # Streamlit application
├── requirements.txt                # Dependencies
├── README.md                       # Project documentation
│
├── assets/
│   └── hdfc_logo.png               # UI assets
│
├── transformer_hdfc_churn_pipeline.pkl
├── target_encoder.pkl
├── Hdfc bank model.pkl
│
└── .devcontainer/                  # Dev container config (optional)
▶️ How to Run the App Locally
1️⃣ Clone the repository
git clone https://github.com/your-username/HDFC-BANK-RETAIL-CREDIT-CARD-CHURN-PREDICTION.git
cd HDFC-BANK-RETAIL-CREDIT-CARD-CHURN-PREDICTION
2️⃣ Create virtual environment (recommended)
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
3️⃣ Install dependencies
pip install -r requirements.txt
4️⃣ Run the Streamlit app
streamlit run app.py
📊 Input Features

The model uses a combination of:

Demographics (gender, city tier)

Employment & income details

Credit behavior

Engagement metrics

Skill & activity indicators

⚠️ Feature names and order strictly match the training schema to prevent silent prediction errors.

✅ Output

Churn Prediction

Yes → Customer likely to churn

No → Customer likely to stay

⚠️ Important Notes

The model will fail intentionally if input schema does not match training schema.

This is a single-customer inference system, not batch prediction.

UI inputs must stay consistent with the trained pipeline.

📌 Future Improvements

Add probability scores for churn risk

Explainability using SHAP

Database integration

Authentication & role-based access

Cloud deployment

👨‍💻 Author

Vivek Shah
AI / ML | Data Science | MLOps
GitHub: vivekshah001

📜 Disclaimer

This project is for educational and demonstration purposes only.
It is not affiliated with or endorsed by HDFC Bank.
