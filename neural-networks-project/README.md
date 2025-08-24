# 🚗 Car Price Prediction: Linear Regression vs Artificial Neural Network

## 📌 Project Overview
This project compares two approaches for predicting car prices:
1. **Linear Regression (Machine Learning)**  
2. **Artificial Neural Network (Deep Learning, TensorFlow/Keras Sequential Model)**  

The goal is to understand how traditional machine learning compares with deep learning when applied to a real-world regression problem.

---

## 📂 Project Structure
- `Car_Price_Prediction_Linear_vs_ANN.ipynb` → Jupyter Notebook with all preprocessing, training, and evaluation steps.
- `data/` → Contains the dataset (if available, otherwise instructions are provided to download it).
- `README.md` → Project documentation.

---

## 🔧 Tools & Libraries
- Python 3.x  
- Pandas, NumPy  
- Matplotlib, Seaborn (visualization)  
- Scikit-learn (Linear Regression, preprocessing)  
- TensorFlow / Keras (Neural Network implementation)

---

## 📊 Steps in the Project
1. **Data Preprocessing**
   - Handle missing values and categorical features.
   - Feature scaling for neural network training.
   - Train/Test split.

2. **Model Training**
   - **Linear Regression** using `sklearn.linear_model`.
   - **ANN** using Keras `Sequential()` with Dense layers.

3. **Evaluation Metrics**
   - Mean Squared Error (MSE)  
   - Mean Absolute Error (MAE)  
   - R² Score  

4. **Visualization**
   - Training/Validation loss curves for the neural network.
   - Comparison plots between predicted vs actual prices.

---

## ✅ Results
- **Linear Regression**: Simple, interpretable, performs well when relationships are linear.  
- **ANN**: Can capture more complex patterns, but requires tuning (layers, neurons, epochs).  
- In this dataset, the performance of ANN vs Linear Regression is compared to highlight trade-offs.

---

---

