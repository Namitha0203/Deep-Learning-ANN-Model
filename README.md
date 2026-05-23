# 🧠 Diabetes Progression Prediction Using Artificial Neural Networks (ANN)

A professional deep learning project implemented in **Google Colab** using **TensorFlow/Keras**, demonstrating how an Artificial Neural Network (ANN) can predict **diabetes disease progression** using clinical features from the scikit‑learn Diabetes dataset.

---

## 📌 Project Summary
This project provides an end‑to‑end workflow for building, training, evaluating, and improving an ANN model for a **regression task**. It covers:

- Data preprocessing  
- Exploratory Data Analysis (EDA)  
- ANN model development  
- Training and validation  
- Performance evaluation  
- Architecture improvement  

The goal is to understand how neural networks learn numerical patterns and how model depth affects performance.

---

## 📂 Dataset
- **Source:** `sklearn.datasets.load_diabetes()`
- **Features:** 10 standardized medical predictors
- **Target:** Continuous disease progression score
- **Missing Values:** None

---

## 🛠️ Technologies Used
- Python  
- TensorFlow / Keras  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  
- Scikit‑learn  

---

## 🔧 Data Preprocessing
- Loaded the Diabetes dataset  
- Verified no missing values  
- Standardized all features using **StandardScaler**  
- Standardization improved:
  - Convergence speed  
  - Gradient stability  
  - Feature balance  

---

## 📊 Exploratory Data Analysis (EDA)
Performed visual analysis to understand data distribution and relationships:

- Histogram of target variable  
- Feature distribution plots  
- Scatter plots showing feature–target relationships  

Insights:
- Target variable is slightly right‑skewed  
- Standardized features are centered and normally distributed  
- Some features show stronger correlation with the target  

---

## 🏗️ ANN Model Architecture

### Initial Model
- Dense(64, activation='relu')  
- Dense(32, activation='relu')  
- Dense(1)  

**Reasoning:**  
Balanced complexity, non‑linear learning capability, suitable for regression.

---

## 🚀 Model Training
- Train/test split: **80% / 20%**
- Loss: **Mean Squared Error (MSE)**
- Optimizer: **Adam**
- Epochs: **100**
- Validation split: **20%**

Training showed consistent reduction in loss and validation loss.

---

## 📈 Model Evaluation

### Initial Model Results
- **MSE:** ~2913  
- **R² Score:** ~0.45  

Interpretation:  
The model explains ~45% of the variance in disease progression.

---

## ⚡ Improved Model

### Improved Architecture
- Dense(128, activation='relu')  
- Dense(64, activation='relu')  
- Dense(32, activation='relu')  
- Dense(1)  

### Improved Results
- **MSE:** ~2789  
- **R² Score:** ~0.47  

✔ Lower error  
✔ Higher accuracy  
✔ Better learning capacity  

---

## 📌 Key Insights
- ANN models can effectively model medical regression tasks  
- Feature scaling is essential  
- Deeper architectures improve performance but require monitoring  
- MSE and R² provide clear evaluation metrics  


---

## ✨ Conclusion
This project demonstrates how to build and optimize an ANN for predicting diabetes progression. It highlights the importance of preprocessing, visualization, model design, and iterative improvement. The comparison between the initial and improved models clearly shows how architectural enhancements can improve predictive performance.



## 📁 Repository Structure

