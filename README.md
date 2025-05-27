# Air-quality-Index-prediction
# AQI Prediction using Random Forest Regressor

This project predicts the **Air Quality Index (AQI)** based on various air pollutants using a machine learning approach. It uses a **Random Forest Regressor** model trained on historical air quality data provided in a ZIP archive (`city_day.csv` inside it). The goal is to evaluate how well air pollutant concentrations can estimate the AQI level.

## 📁 Dataset

The dataset used is the `city_day.csv` file, typically provided in a compressed `.zip` format. It includes daily readings of multiple pollutants from different Indian cities and corresponding AQI values.

**Features used for prediction:**
- PM2.5
- PM10
- NO
- NO2
- NOx
- NH3
- CO
- SO2
- O3
- Benzene
- Toluene

**Target:**
- AQI (Air Quality Index)

## 🧪 Tech Stack

- Python 3
- Pandas
- Matplotlib & Seaborn (for visualization)
- Scikit-learn (for ML model and evaluation)
- Google Colab (for notebook execution)
- Random Forest Regressor

## 🚀 How It Works

1. **Upload ZIP File**: The user uploads a `.zip` containing `city_day.csv`.
2. **Extract and Load Data**: The code extracts the file and reads the dataset into a DataFrame.
3. **Data Preprocessing**:
   - Drops rows with missing values.
   - Selects relevant feature columns.
   - Scales features using `StandardScaler`.
4. **Model Training**: Uses `RandomForestRegressor` to fit on training data.
5. **Evaluation**:
   - Calculates Mean Squared Error (MSE) and R² score.
   - Visualizes actual vs. predicted AQI using a scatter plot.

## 📊 Output

- **MSE** and **R² Score**: Printed in the console.
- **Scatter Plot**: Displays comparison between actual and predicted AQI values.

## 🧠 Requirements

Make sure the following Python libraries are installed:
```bash
pip install pandas matplotlib seaborn scikit-learn
