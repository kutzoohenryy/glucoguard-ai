# 🩺 GlucoGuard AI — Diabetes Risk Prediction

**An AI-powered educational web application for understanding potential diabetes risk.**

GlucoGuard AI is a machine learning-based web application that estimates potential diabetes risk using health-related inputs. It combines a Python Flask backend, a React frontend, and a machine learning pipeline to present model predictions and health insights in an accessible, user-friendly interface.

> **Disclaimer:** GlucoGuard AI is an educational project and is not intended for medical diagnosis, treatment, or clinical decision-making. Its predictions are not clinically validated. Always consult a qualified healthcare professional for medical advice.

## ✨ Features

- **AI-Based Risk Prediction:** Uses a trained machine learning model to estimate potential diabetes risk.
- **Interactive Health Assessment:** Allows users to enter health-related information for assessment.
- **Easy-to-Understand Insights:** Presents results in a more accessible format rather than only displaying technical ML outputs.
- **Health Awareness:** Helps users explore factors such as glucose, blood pressure, and BMI.
- **Interactive Dashboard:** Built with React for a responsive and engaging user experience.
- **REST API:** Flask backend handles prediction requests.
- **Model Evaluation:** Includes metrics to assess model performance.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Backend and machine learning |
| Flask | REST API |
| React | Frontend user interface |
| Vite | Frontend development server |
| Scikit-learn | Machine learning pipeline |
| Pandas & NumPy | Data processing |
| Recharts | Data visualization |
| Lucide React | UI icons |
| Joblib | Saving and loading the trained model |

## 🧠 Machine Learning Model

The project uses a **Logistic Regression** model trained on a diabetes dataset.

### Model Performance

| Metric | Result |
|---|---:|
| Accuracy | 73.38% |
| Precision | 60.32% |
| Recall | 70.37% |
| Specificity | 75.00% |
| F1 Score | 64.96% |
| ROC-AUC | 82.48% |

These metrics reflect evaluation on the project's test split. They do not establish clinical reliability or guarantee accurate predictions for individual users.

## 📂 Project Structure

```text
glucoguard-ai/
├── backend/
│   └── ...                  # Flask API
├── frontend/
│   └── ...                  # React + Vite application
├── data/
│   └── diabetes.csv         # Dataset, subject to its licence
├── models/
│   ├── glucoguard_pipeline.joblib
│   └── model_metadata.json
├── requirements.txt
└── README.md
```

*Note: This structure describes the main project components. Your actual folders may contain additional files.*

## 🚀 Getting Started

### Prerequisites

Install the following before running the project:

- Python 3.10 or a compatible version for your dependencies
- Node.js and npm
- Git (optional, for cloning the repository)

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/GlucoGuard-AI.git
cd GlucoGuard-AI
```

Replace `YOUR-USERNAME` with your GitHub username.

### 2. Set Up the Backend

Open a terminal in the project root:

```bash
python -m venv .venv
```

Activate the virtual environment.

**Windows PowerShell:**

```powershell
.\.venv\Scripts\Activate.ps1
```

Install Python dependencies:

```bash
pip install -r requirements.txt
```

Start the Flask backend using the entry-point file in your `backend` folder. For example, if the file is named `app.py`:

```bash
python backend/app.py
```

The backend health check should be available at:

```text
http://127.0.0.1:5000
```

### 3. Start the Frontend

Open a **second terminal**:

```bash
cd frontend
npm install
npm run dev
```

Open the local URL printed by Vite, usually:

```text
http://localhost:5173
```

Keep both terminal processes running while using the application.

> If your Flask entry-point filename or API routes differ, use the actual names in your project.

## 📊 Evaluation Metrics

The model is evaluated using multiple metrics because accuracy alone does not describe all prediction errors.

- **Accuracy:** Overall proportion of correct predictions.
- **Precision:** Proportion of predicted positive cases that were actually positive in the test data.
- **Recall:** Proportion of actual positive cases identified by the model.
- **Specificity:** Proportion of actual negative cases correctly identified.
- **F1 Score:** Balance between precision and recall.
- **ROC-AUC:** Measures how well the model ranks positive cases above negative cases across classification thresholds.

## 🔮 Future Improvements

- Add more extensive model validation and calibration.
- Improve accessibility and mobile responsiveness.
- Add clearer explanations of individual predictions.
- Expand automated testing and API error handling.
- Evaluate the model on more representative datasets.
- Add privacy-conscious handling of user inputs.
- Deploy the application for demonstration purposes.

## 🎯 Project Objective

The objective of GlucoGuard AI is to explore how machine learning, web development, and health data can be combined to build an accessible educational application.

This project demonstrates practical skills in **Python, machine learning, REST APIs, React, data analysis, and model evaluation**.

## 👨‍💻 Author

**Rishabh Singh**

B.Tech — Computer Science Engineering, Data Science

LinkedIn: [Connect with me](https://www.linkedin.com/in/rishabh-singh-46890b326)

## 📄 License

No licence has been specified yet. Add a licence file if you intend to permit others to reuse, modify, or distribute the project. Also verify the dataset's licence before redistributing it.

---

⭐ If you find this project interesting, feel free to explore the repository and share feedback.
