#  Crop Recommendation System

[![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-Web%20App-green?logo=flask)](https://flask.palletsprojects.com/)
[![Scikit-learn](https://img.shields.io/badge/ML-Scikit--learn-orange?logo=scikit-learn)](https://scikit-learn.org/)
[![NumPy](https://img.shields.io/badge/NumPy-Data%20Processing-yellow?logo=numpy)](https://numpy.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-red?logo=pandas)](https://pandas.pydata.org/)

> An intelligent crop recommendation web application built with Flask and Machine Learning. Input soil and weather parameters to get instant crop suggestions powered by a trained Random Forest model.



##  Table of Contents

- [About the Project](#-about-the-project)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Screenshots](#-screenshots)
- [Installation](#-installation)
- [Usage](#-usage)
- [Project Structure](#-project-structure)
- [How It Works](#-how-it-works)
- [Contributing](#-contributing)

---

## About the Project

The **Crop Recommendation System** is a full-stack machine learning application that helps farmers make data-driven decisions about crop selection. By analyzing key soil nutrients (Nitrogen, Phosphorus, Potassium) along with environmental factors (Temperature, Humidity, pH, Rainfall), the system predicts the most suitable crop to grow.

This project demonstrates the integration of:
- **Machine Learning** (Random Forest Classifier)
- **Web Development** (Flask backend + Bootstrap UI)
- **Data Preprocessing** (StandardScaler + MinMaxScaler)
- **Model Serialization** (joblib for persistence)



## Features

- 🌾 Predicts **22 different crops** based on soil and climate data
- 🎨 Clean, responsive **Bootstrap-based web interface**
- ⚙️ **Dual-scaling pipeline** (MinMax + Standard Scaler) for optimal model performance
- 📦 **Pre-trained model** with saved scalers for instant deployment
- 🐞 Built-in **error handling** with user-friendly feedback
- 📁 **Jupyter Notebook** included for model training and experimentation



## Tech Stack

| Category | Technology |
|----------|------------|
| Backend | Python, Flask |
| Machine Learning | Scikit-learn (Random Forest) |
| Data Processing | NumPy, Pandas |
| Model Serialization | joblib |
| Frontend | HTML5, CSS3, Bootstrap |



## Screenshots

### Input Form
![Input Form](screenshots/form.png)

### Prediction Output
![Prediction Output](screenshots/predictionOutput.png)



## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/tanu-dev0/Crop-Recommendation-System.git
cd Crop-Recommendation-System
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

**Windows:**
```bash
venv\Scripts\activate
```

**Linux/Mac:**
```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️Usage

### Running the Web Application

```bash
python app.py
```

Open your browser and navigate to: **http://127.0.0.1:5000/**

### Input Parameters

| Parameter | Description | Unit |
|-----------|-------------|------|
| Nitrogen | Nitrogen content in soil | mg/kg |
| Phosphorus | Phosphorus content in soil | mg/kg |
| Potassium | Potassium content in soil | mg/kg |
| Temperature | Ambient temperature | °C |
| Humidity | Relative humidity | % |
| pH | Soil pH level | 0-14 |
| Rainfall | Annual rainfall | mm |

---

## 📂 Project Structure

```
Crop-Recommendation-System/
├── app.py                      # Flask web application
├── requirements.txt            # Python dependencies
├── Crop_Recommendation_System.ipynb   # Model training notebook
├── Crop_recommendation.csv     # Training dataset
├── model.pkl                   # Trained Random Forest model
├── standscaler.pkl             # StandardScaler
├── minmaxscaler.pkl            # MinMaxScaler
├── templates/
│   └── index.html              # Web interface
└── screenshots/
    ├── form.png                # Input form screenshot
    └── predictionOutput.png    # Prediction result screenshot
```

---

## 🧠 How It Works

1. **Data Preprocessing** - Input features are normalized using MinMaxScaler, then standardized using StandardScaler for optimal model performance.
2. **Model Prediction** - A pre-trained Random Forest Classifier processes the scaled features and outputs a predicted crop class.
3. **Result Mapping** - The numeric prediction is mapped to a human-readable crop name (e.g., Rice, Maize, Cotton).
4. **Web Display** - The result is displayed on the web interface with a success message.

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repository and submit pull requests.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

<div align="center">

**Made with ❤️ by [tanu-dev0](https://github.com/tanu-dev0)**

[![GitHub](https://img.shields.io/badge/GitHub-View%20Profile-black?logo=github)](https://github.com/tanu-dev0)

</div>
```

