# 🚗 Car Price Prediction using Machine Learning

A machine learning project that predicts the **price of a car** based on its specifications such as brand, manufacturing year, fuel type, body type, transmission, horsepower, and other vehicle features.

The project includes **data preprocessing, exploratory data analysis (EDA), feature engineering, model training, hyperparameter tuning, performance evaluation, and model serialization** for future deployment.

---

## 📌 Features

* 📊 Exploratory Data Analysis (EDA)
* 🧹 Data Cleaning & Preprocessing
* 🔤 Label Encoding for categorical features
* ⚙️ Feature Engineering
* 📈 Multiple Regression Models
* 🎯 Hyperparameter Tuning
* 📉 Model Performance Comparison
* 💾 Model Export using Pickle
* 🚀 Ready for deployment with Flask, FastAPI, or Streamlit

---

## 🛠️ Tech Stack

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Pickle

---

## 📂 Project Structure

```text
Car-Price-Prediction/
│
├── prediction.ipynb              # Complete notebook
├── global_cars_enhanced.csv      # Dataset
├── car_price_model.pkl           # Saved trained model
├── requirements.txt
├── README.md
└── images/
    └── model_comparison.png      # (Optional)
```

---

## 📊 Dataset

The dataset contains information about different cars, including:

| Feature               | Description                          |
| --------------------- | ------------------------------------ |
| Brand                 | Car manufacturer                     |
| Manufacture_Year      | Manufacturing year                   |
| Fuel_Type             | Petrol, Diesel, Hybrid, Electric     |
| Transmission          | Manual / Automatic                   |
| Body_Type             | Sedan, SUV, Hatchback, Coupe, Pickup |
| Horsepower            | Engine power                         |
| Engine_CC             | Engine displacement                  |
| Manufacturing_Country | Country of origin                    |
| Mileage_km_per_l      | Fuel efficiency                      |
| Efficiency_Score      | Efficiency rating                    |
| Price_Category        | Budget, Mid-Range, Premium, Luxury   |
| Age_Category          | New, Recent, Moderate, Old           |
| Price_USD             | Original target price                |
| Price                 | Processed target variable            |

---

# 📈 Exploratory Data Analysis

The notebook performs:

* Dataset overview
* Missing value analysis
* Feature distributions
* Category analysis
* Statistical summaries
* Count plots for categorical features

---

# ⚙️ Data Preprocessing

The following preprocessing steps are applied:

* Missing value checking
* Label Encoding for categorical columns
* Feature scaling using `StandardScaler`
* Feature selection
* Train-Test split (80/20)

Categorical columns encoded:

* Brand
* Fuel_Type
* Transmission
* Body_Type
* Manufacturing_Country
* Price_Category
* Age_Category

---

# 🤖 Machine Learning Models

The following regression algorithms are trained and compared:

* Linear Regression
* Random Forest Regressor
* AdaBoost Regressor
* Gradient Boosting Regressor

---

# 📏 Evaluation Metrics

Each model is evaluated using:

* R² Score
* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)

Example comparison:

| Model             | R² Score | MAE    | RMSE   |
| ----------------- | -------- | ------ | ------ |
| AdaBoost          | Highest  | Lowest | Lowest |
| Random Forest     | High     | Low    | Low    |
| Gradient Boosting | High     | Low    | Low    |
| Linear Regression | Baseline | Higher | Higher |

---

# 💾 Model Saving

The best-performing model is saved along with:

* Trained model
* StandardScaler
* Label Encoders

```python
pickle.dump(artifacts, open("car_price_model.pkl", "wb"))
```

This makes the project deployment-ready.

---

# 🚀 Installation

Clone the repository:

```bash
git clone http://github.com/AnujrajShrestha/car_price_prediction

cd car_price_prediction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# ▶️ Run the Project

Open the notebook:

```bash
jupyter notebook prediction.ipynb
```

Run all cells sequentially.

---

# 🔮 Example Prediction Inputs

```text
Brand: Toyota
Manufacture Year: 2022
Body Type: SUV
Fuel Type: Petrol
Transmission: Automatic
Engine CC: 1800
Horsepower: 140
Price Category: Premium
Age Category: Recent
```

The model predicts the estimated car price based on these features.

---

# 📚 Libraries Used

```text
numpy
pandas
matplotlib
seaborn
scikit-learn
pickle
```

---

# 🔥 Future Improvements

* Build a Streamlit web application
* Add FastAPI backend
* Dockerize the project
* Deploy on Render or Hugging Face Spaces
* Integrate SHAP for model explainability
* Automate hyperparameter optimization with Optuna
* Add CI/CD pipeline with GitHub Actions

---

# 👨‍💻 Author

**Anuj Shrestha**

* GitHub: [https://github.com/AnujrajShrestha](https://github.com/AnujrajShrestha)

---

## ⭐ If you found this project useful, consider giving it a star on GitHub!
