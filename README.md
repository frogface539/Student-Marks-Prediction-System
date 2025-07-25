# 🎓 Student Average Score Prediction App

An interactive machine learning web app that predicts a student's **average exam score** using **AdaBoost** and **Gradient Boosting** regression models. Built with a vibrant **Streamlit** UI and dynamic **Plotly** visualizations.

---

## 🚀 Key Features

* 📊 **Predicts Average Score** using:

  * Math, Reading, and Writing scores
  * Gender, Ethnicity
  * Parental education level
  * Lunch type
  * Test preparation course

* 🔁 **Compare Two Models**:

  * 🔹 AdaBoost Regressor
  * 🔸 Gradient Boosting Regressor

* 🎯 **Score Classification**:

  * **Fail**: score < 50
  * **Average**: score 50–75
  * **Excellent**: score > 75

* 📈 Interactive **Plotly radial gauges**

* 🎨 Clean and emoji-powered **Streamlit UI**

---

## 💻 Demo

> 🌐 [Deployed](https://youtu.be/your-demo-link)

---

## 🧠 ML Pipeline Overview

### 1. **Data Preprocessing**

* Cleaned column names
* One-hot encoded categorical features
* Created target: `average_score = (math + reading + writing) / 3`

### 2. **Model Training**

* Models used:

  * `AdaBoostRegressor`
  * `GradientBoostingRegressor`
* Hyperparameter tuning via `RandomizedSearchCV`

### 3. **Evaluation**

* Metrics: **R²**, **MAE**, **MSE**
* Saved best models using `pickle`

### 4. **Deployment**

* Built with **Streamlit** + **Plotly**
* Inputs: sliders, dropdowns, radio buttons
* Output: numeric prediction + score class + radial gauge

---

## 📦 Project Structure

```
student-score-prediction/
├── app.py                 # Streamlit web app
├── utils.py               # Preprocessing and prediction logic
├── models/
│   ├── adaboost_model.pkl
│   └── gradient_model.pkl
├── requirements.txt       # Project dependencies
└── README.md
```

---

## 📊 Dataset

* 📁 Source: [Student Performance in Exams – Kaggle](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
* Size: 1000 records
* Target: `average_score`

---

## 🛠 Tech Stack

* `Python`
* `scikit-learn` — modeling and evaluation
* `pandas`, `numpy` — data processing
* `Streamlit` — frontend UI
* `Plotly` — score gauges
* `pickle` — model serialization

---

## 🚀 How to Run Locally

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/student-score-prediction.git
   cd student-score-prediction
   ```

2. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Streamlit app**:

   ```bash
   streamlit run app.py
   ```

---

## 👤 Author

**Lakshay Jain**
🔗 [LinkedIn](https://www.linkedin.com/in/lakshay-jain-a48979289/)
🐙 [GitHub](https://github.com/frogface539)

> ⭐ Star this repo if you find it useful! Contributions and feedback are always welcome.

---