# 🏦 Loan Approval Prediction

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-1.53.1-FF4B4B?logo=streamlit&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.8.0-F7931E?logo=scikit-learn&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)
![Live App](https://img.shields.io/badge/Live%20App-Streamlit-brightgreen)

A machine learning web application that predicts whether a loan application will be **approved or rejected** based on applicant financial and personal details. Built with Python, scikit-learn, and deployed using Streamlit Cloud.

🔗 **Live Demo:** [https://loanapprovalprediction-lqrymmlujf4xasg3hjfq6g.streamlit.app/](https://loanapprovalprediction-lqrymmlujf4xasg3hjfq6g.streamlit.app/)

---

## 📌 Project Overview

Loan approval is a critical process in the banking and financial sector. This project automates that decision-making process using a trained machine learning classification model. The user inputs applicant details through an interactive web form, and the model instantly predicts whether the loan would be approved or rejected.

---

## 🚀 Features

- **Interactive Web App** — Clean Streamlit UI with real-time prediction
- **ML-Powered Predictions** — Trained classification model serialized as `model.pkl`
- **11 Input Features** — Covers financial and demographic attributes
- **Instant Results** — Displays ✅ Loan Approved or ❌ Loan Rejected on button click
- **Deployed on Streamlit Cloud** — Accessible from any browser without local setup

---

## 🧠 Input Features

| Feature | Type | Description |
|---|---|---|
| Applicant Income | Numeric | Monthly income of the primary applicant |
| Coapplicant Income | Numeric | Monthly income of the co-applicant |
| Loan Amount | Numeric | Requested loan amount (in thousands) |
| Loan Amount Term | Numeric | Repayment term in months |
| Credit History | Categorical | 1.0 = Good credit history, 0.0 = Bad |
| Gender | Categorical | Male / Female |
| Married | Categorical | Yes / No |
| Dependents | Categorical | 0, 1, 2, 3+ |
| Education | Categorical | Graduate / Not Graduate |
| Self Employed | Categorical | Yes / No |
| Property Area | Categorical | Urban / Semiurban / Rural |

---

## 🗂️ Project Structure

```
Loan_Approval_Prediction/
│
├── Loan_Approval_Prediction.ipynb  # EDA, preprocessing & model training notebook
├── streamlit_app.py                # Streamlit web application
├── model.pkl                       # Trained ML model (serialized with pickle)
├── loan_approved.csv               # Dataset used for training
├── requirements.txt                # Python dependencies
└── README.md                       # Project documentation
```

---

## 🔧 Tech Stack

| Layer | Technology |
|---|---|
| Language | Python 3.10+ |
| ML Library | scikit-learn |
| Data Processing | pandas, numpy |
| Visualization | matplotlib, seaborn |
| Web Framework | Streamlit |
| Model Serialization | pickle |
| Deployment | Streamlit Cloud |

---

## 📊 Workflow

1. **Data Collection** — Used the `loan_approved.csv` dataset containing historical loan application data
2. **Exploratory Data Analysis (EDA)** — Analyzed distributions, missing values, correlations, and feature relationships
3. **Data Preprocessing** — Handled missing values, encoded categorical variables, and scaled numerical features
4. **Model Training** — Trained a classification model using scikit-learn and evaluated performance metrics
5. **Model Serialization** — Saved the trained model as `model.pkl` using pickle
6. **Web App Development** — Built an interactive Streamlit app for real-time predictions
7. **Deployment** — Deployed the app on Streamlit Cloud for public access

---

## 💻 Run Locally

### Prerequisites
- Python 3.10 or higher
- pip

### Steps

```bash
# 1. Clone the repository
git clone https://github.com/Vasanth4321/Loan_Approval_Prediction.git
cd Loan_Approval_Prediction

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the Streamlit app
streamlit run streamlit_app.py
```

The app will open in your browser at `http://localhost:8501`

---

## 📷 App Preview

The app accepts the following inputs and returns a prediction:

- Fill in numerical inputs: Applicant Income, Coapplicant Income, Loan Amount, Loan Amount Term, Credit History
- Select categorical inputs: Gender, Married, Dependents, Education, Self Employed, Property Area
- Click **"Predict Loan Status"** to get the result

---

## 📁 Dataset

The dataset `loan_approved.csv` contains loan application records with the following target variable:

- **Loan_Status** — `Y` (Approved) / `N` (Rejected)

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/Vasanth4321/Loan_Approval_Prediction/issues).

---

## 👤 Author

**Venkata Sai Vasanth Neeli**
- GitHub: [@Vasanth4321](https://github.com/Vasanth4321)
- LinkedIn: [Connect on LinkedIn](https://www.linkedin.com/in/venkata-sai-vasanth-neeli/)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
