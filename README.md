## 🧠 Machine Learning Projects

This repository showcases several **machine learning notebooks** focused on classification, regression, and data preprocessing using real-world datasets from **Kaggle** and **Google Drive**.

---

## 📂 Project Structure

```
📁 ML_Projects

├── 2D point dataset.ipynb                     # 🔹 Beginner ML on 2D data

├── Churn_prediction ML project.ipynb          # 🔥 Customer churn classification

├── Different Models of ML.ipynb               # 📈 Model comparison on stock data

├── Hand_Written_Dataset Recognition.ipynb     # ✍️ Digit classification (likely MNIST)

├── SVM on Multiple CSVs.ipynb                 # ⚽ Regression on FIFA datasets (SVM)

├── .gitkeep
```

---

## 🔍 Project Overviews

### 📌 1. **SVM on FIFA Multi-Year Dataset**

* Loads `players_15.csv` to `players_20.csv` and `teams_and_leagues.csv` using Kaggle API
* Merges data and applies extensive cleaning + `LabelEncoder`
* Predicts `overall` player rating using `SVR` (Support Vector Regression)

---

### 📌 2. **Churn Prediction (Telco Dataset)**

* Binary classification using Google Drive dataset
* Replaces categorical columns with 0/1 or one-hot encodings
* Applies various models (`LinearRegression`, `Ridge`, `Lasso`, `RandomForestRegressor`)
* Identifies best performer based on **MAE**

---

### 📌 3. **Stock Exchange Dataset (Multi-CSV Merge)**

* Combines `fundamentals.csv`, `securities.csv`, `prices.csv`, and `prices-split-adjusted.csv`
* Drops redundant columns and fills missing values
* Performs regression on the stock market dataset using:

  * `LinearRegression`, `Lasso`, `Ridge`, `RandomForestRegressor`, `GradientBoostingRegressor`
* Evaluates models using **MSE** to select the best regressor

---

### 📌 4. **Handwritten Digit Recognition**

* Image classification task using hand-written dataset (likely MNIST)
* Implements classification using scikit-learn or TensorFlow models
* Emphasis on image preprocessing, training, and performance evaluation

---

### 📌 5. **2D Point Dataset Classification**

* A minimal example showcasing a classifier applied to a 2D dataset
* Good for beginners to understand data separation and decision boundaries

---

## 💻 Requirements

Install essential dependencies:

```bash
pip install pandas numpy scikit-learn tensorflow matplotlib kaggle
```

Or in Google Colab:

```python
!pip install -q kaggle
!pip install -q tensorflow
!pip install -q scikit-learn pandas
from google.colab import drive
drive.mount('/content/drive')
```

To download from Kaggle:

```bash
# Upload kaggle.json first
!mkdir ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
!kaggle datasets download -d stefanoleone992/FIFA-20-complete-player-dataset
```

---

## 🔑 Key Skills Demonstrated

✔️ Data preprocessing (handling NaN, encoding, merging CSVs)

✔️ Regression and classification model building

✔️ Model evaluation: MSE, MAE, prediction visualizations

✔️ Kaggle + Google Drive integration in Colab

✔️ Comparative analysis of scikit-learn models

✔️ End-to-end ML pipeline building

---

## 🚀 Use Cases

* 📊 Predicting player performance from FIFA historical data
* 🔍 Identifying churn patterns for customer retention
* 📈 Stock trend modeling using multi-source financial data
* ✍️ Digit recognition for image classification projects
* 📐 Foundation building for classification and regression tasks

---
