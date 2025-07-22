
# ❤️ Heart Failure Prediction Web App

This is a simple Flask-based web application that predicts the likelihood of heart failure using a machine learning model trained on clinical data. The model was trained in **Google Colab**, and the web application was developed and tested using **PyCharm** on macOS.

---

## 🧠 Machine Learning Model

The model used is a **Random Forest Classifier** trained on clinical data including:

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

The trained model is saved as `model.pkl` using `joblib`.

---

## 🖥️ Tech Stack

- Python 3  
- Scikit-learn  
- Joblib  
- Flask  
- HTML & CSS (custom styles)  

---

## 📂 Project Structure

```
HeartFailurePrediction/
├── app.py
├── model.pkl
├── heart_failure_model.ipynb
├── requirements.txt
├── README.md
└── templates/
    └── index.html
```

---

## 🚀 Running the Project Locally on macOS

### 🧰 Step-by-Step Setup:

1. **Clone or download** the repository:
```bash
git clone https://github.com/yourusername/HeartFailurePrediction.git
cd HeartFailurePrediction
```

2. **Create and activate a virtual environment**:
```bash
python3 -m venv venv
source venv/bin/activate
```

3. **Install dependencies**:
```bash
pip install -r requirements.txt
```

4. **Run the Flask app**:
```bash
python app.py
```

5. Open your browser and go to `http://127.0.0.1:5000`

---

## 🔍 How Prediction Works

You can input patient health metrics into the web form, and the app will respond with:

- ✅ **No Heart Disease Detected**
- ❌ **Heart Disease Detected**

This is determined by the Random Forest model’s prediction.

---

## ☁️ Training the Model in Google Colab

1. Upload the dataset and the training notebook (`heart_failure_model.ipynb`) to your Colab.
2. Train the model and export it using:
```python
import joblib
joblib.dump(model, 'model.pkl')
```
3. Download `model.pkl` and move it to your Flask app folder locally.

---

## 💻 Screenshots

<img width="1440" height="900" alt="Screenshot 1" src="https://github.com/user-attachments/assets/fc71f41b-f352-4201-8752-c931f9d883f1" />
<img width="1440" height="900" alt="Screenshot 2" src="https://github.com/user-attachments/assets/5ef6692e-cedf-4197-90ad-463fa2b799cd" />

---

## 🔐 Notes

> This is a development app. For production, use a proper WSGI server like Gunicorn and secure the app with HTTPS.

---

## 🏁 Developed For

This project was created as part of a **Machine Learning Bootcamp** assignment, focusing on real-world deployment of ML models using Flask.
