# Heart Failure Prediction Web App

This is a simple Flask-based web application that predicts the likelihood of heart failure using a machine learning model trained on health data.

## 🧠 Model

The model used is a **Random Forest Classifier** trained on clinical data such as:
- Age
- Gender
- Chest Pain Type
- Resting Blood Pressure
- Cholesterol
- Fasting Blood Sugar
- ECG Results
- Maximum Heart Rate Achieved
- Exercise-induced Angina
- ST Depression
- Slope of the Peak Exercise ST Segment
- Number of Major Vessels Colored
- Thalassemia

Model is saved as `model.pkl`.

## 🖥️ Tech Stack

- Python 3
- Flask
- HTML/CSS
- Scikit-learn
- Joblib

## 📂 Project Structure

```
HeartFailureApp/
├── app.py
├── model.pkl
├── templates/
│   └── index.html
└── README.md
```

## 🚀 Running Locally

1. Clone or download this repository
2. Navigate to the project folder
3. Install required packages:

```bash
pip install flask joblib scikit-learn
```

4. Start the app:

```bash
python app.py
```

5. Open your browser and go to `http://127.0.0.1:5000`

## 🔍 Prediction

Input patient features on the homepage form. Based on the model prediction, it will return:
- **Heart Disease Detected** or
- **No Heart Disease Detected**

## 📸 Screenshots

Feel free to add screenshots of the interface here.

---

Developed as part of a machine learning bootcamp project.
