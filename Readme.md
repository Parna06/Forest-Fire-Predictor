
# 🌲 Forest Fire Weather Index (FWI) Prediction App

A **Machine Learning-powered web application** built using **Flask**, designed to predict the **Forest Fire Weather Index (FWI)** based on key meteorological and environmental parameters.  

This project integrates data analysis, feature engineering, and model training with an intuitive front-end interface — helping users estimate fire risk levels quickly and accurately.  

---

## 🚀 Features

- 🧠 **ML Model Integration** – Ridge Regression model for FWI prediction.  
- ⚙️ **Feature Scaling** – Data is standardized using `StandardScaler` for optimal prediction accuracy.  
- 🌦️ **Interactive Web Form** – Input temperature, humidity, wind speed, and other parameters to get instant predictions.  
- 🖥️ **Simple Flask Interface** – Lightweight and fast, built with `Flask` and served with dynamic templates.  
- 📊 **Data-Driven Insights** – Model trained through extensive **EDA (Exploratory Data Analysis)** and **Feature Engineering**.  

---

## 🧩 Tech Stack

| Component | Technology |
|------------|-------------|
| **Frontend** | HTML5, CSS3 |
| **Backend** | Python, Flask |
| **Machine Learning** | Scikit-learn (Ridge Regression, StandardScaler) |
| **Data Handling** | NumPy, Pandas |
| **Model Files** | Pickled `.pkl` model and scaler |
| **Templates** | Jinja2-based HTML forms |

---

## 🧪 How It Works

1. **User Input** – Enter environmental parameters such as:
   - Temperature  
   - Relative Humidity (RH)  
   - Wind Speed (Ws)  
   - Rain  
   - FFMC, DMC, ISI  
   - Classes  
   - Region  

2. **Data Preprocessing** – Input data is transformed using the pre-trained `StandardScaler`.

3. **Prediction** – The processed data is passed to the trained Ridge Regression model to predict FWI.

4. **Output Display** – The result is rendered dynamically on the **Home page**.

---

## 📁 Project Structure

```
├── application.py           # Flask backend and routing
├── templates/
│   ├── index.html           # Landing page
│   ├── home.html            # Prediction page
├── models/
│   ├── ridge.pkl            # Trained Ridge Regression model
│   └── scaler.pkl           # StandardScaler object
├── notebooks/
│   ├── EDA and FE.ipynb     # Exploratory Data Analysis and Feature Engineering
│   └── model_training.ipynb # Model training notebook
└── README.md                # Project documentation
```

---

## ⚡ Getting Started

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/fwi-prediction-app.git
cd fwi-prediction-app
```

### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Application
```bash
python application.py
```

### 4️⃣ Access the App
Visit 👉 **http://127.0.0.1:5000/** in your browser.

---

## 🧠 Model Training Overview

The predictive model was trained using Ridge Regression, after performing:
- Exploratory Data Analysis (EDA)
- Feature Engineering (FE)
- Data Scaling
- Model Evaluation using RMSE and R² metrics  

For a deeper understanding, refer to the notebooks:
- `EDA and FE.ipynb`
- `model_training.ipynb`

---

## 🌐 Web Pages Overview

- **index.html** – Landing page introducing the app.  
- **home.html** – Input form and result display.  

---

## 📸 Preview

**Home Page Form**
```
Enter the required parameters ➜ Click Predict ➜ Get the FWI instantly!
```

