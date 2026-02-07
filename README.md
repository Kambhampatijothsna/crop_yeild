# 🌾 Crop Yield Prediction using Machine Learning

This project focuses on predicting **Crop Yield (hg/ha)** using **Machine Learning regression models** based on various agricultural and environmental factors such as rainfall, temperature, pesticide usage, crop type, and region/country.

The main objective of this project is to help in understanding how different factors influence crop yield and to build a model that can predict yield accurately using historical data.

---

## 📌 Project Overview

Crop yield prediction is an important task in agriculture as it helps:

- Farmers to plan crop cultivation effectively  
- Governments to estimate food production  
- Researchers to analyze agricultural patterns  
- Policymakers to make data-driven decisions  

This project uses a dataset containing crop yield data across multiple countries, crops, and years. Several regression models are trained and compared to select the best-performing model.

---

## 📂 Dataset Information

The dataset contains the following columns:

| Column Name | Description |
|------------|-------------|
| `Area` | Country/Region name |
| `Item` | Crop name (e.g., Wheat, Rice, Sorghum) |
| `Year` | Year of record |
| `hg/ha_yield` | Crop yield (Target column) |
| `average_rain_fall_mm_per_year` | Average rainfall per year |
| `pesticides_tonnes` | Pesticide usage in tonnes |
| `avg_temp` | Average temperature |

🎯 **Target Variable:** `hg/ha_yield`

---

## ⚙️ Technologies Used

- Python  
- Google Colab / Jupyter Notebook  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Machine Learning Regression Models  

---

## 🧠 Machine Learning Models Used

The following regression models were trained and compared:

- Random Forest Regressor  
- K-Nearest Neighbors (KNN)  
- Decision Tree Regressor  
- Bagging Regressor  
- Bayesian Ridge Regression  
- Linear Regression (if included)  
- Ridge / Lasso Regression (if included)  

---

## 📊 Model Evaluation Metrics

The models were evaluated using the following performance metrics:

- **MAE (Mean Absolute Error)**  
- **MSE (Mean Squared Error)**  
- **RMSE (Root Mean Squared Error)**  
- **R² Score (Coefficient of Determination)**  

---

## 📌 Example Prediction Output

Example input:

- Crop: **Wheat**  
- Country: **India**  
- Year: **2023**  

Example output:

**Predicted Crop Yield:** 22067.54 hg/ha  

---

## 📊 Results

The best-performing model was selected based on the highest **R² Score** and lowest error values.

### Example Model Comparison Table

| Model | MAE | RMSE | R² Score |
|------|------|------|----------|
| Random Forest | 3713.40 | 9384.34 | 0.9877 |
| Bayesian Ridge | 3990.92 | 10136.62 | 0.9857 |
| KNN | 4611.26 | 10396.80 | 0.9849 |

✅ **Best Model:** Random Forest Regressor (Based on R² Score)

---

## 🚀 How to Run the Project

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Kambhampatijothsna/crop_yeild.git
```

### 2️⃣ Navigate to the Project Folder
cd crop_yeild

### 3️⃣ Install Dependencies
pip install -r requirements.txt

### 4️⃣ Run the Notebook

Open the notebook file in Jupyter Notebook or Google Colab and execute all cells:

crop_yield_prediction.ipynb

## 📁 Project Structure

```bash
📦 crop_yeild
 ┣ 📜 crop_yield_prediction.ipynb
 ┣ 📜 dataset.csv
 ┣ 📜 README.md
 ┣ 📜 requirements.txt
