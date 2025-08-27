# 🧠 CNN vs ANN on MNIST

## 📌 Overview  
This project presents a comparison between two models for classifying handwritten digit images (MNIST):  
- **Convolutional Neural Network (CNN)**  
- **Artificial Neural Network (ANN/MLP)**  

The goal is to analyze the impact of network architecture on **accuracy** and **training performance**.

---

## 🗂️ Dataset  
- **Source**: Keras Library
- **Samples**: 60,000 for training + 10,000 for testing  
- **Image format**: 28×28 grayscale  
- **Preprocessing**:  
  - Normalization to [0, 1]  
  - Reshaping to fit each model’s input  

---

## ⚙️ Models

### 🔹 ANN (Multi-Layer Perceptron)  
- Flatten layer (784 input features)  
- Dense(128, ReLU)  
- Dropout(0.3)  
- Dense(10, Softmax)  

### 🔹 CNN  
- Conv2D(32 filters, 3×3, ReLU) + MaxPooling(2×2)  
- Conv2D(64 filters, 3×3, ReLU) + MaxPooling(2×2)  
- Conv2D(64 filters, 3×3, ReLU)  
- Flatten  
- Dense(64, ReLU)  
- Dense(10, Softmax)  

---

## 🏋️ Training  
- **Optimizer**: RMSprop  
- **Loss Function**: Categorical Crossentropy  
- **Metrics**: Accuracy  
- **Epochs**: 5 (can be tuned)  
- **Batch size**: 64  

---

## 📊 Results (Summary)  
> Results may slightly vary depending on hardware and number of epochs.

- **CNN**: Higher accuracy (~99%)  
- **ANN**: Lower accuracy (~97%)  

The CNN clearly outperforms the ANN thanks to its ability to extract spatial features from images.  

---

## 🚀 How to Run  
```bash
git clone <repo-url>
cd <repo-name>
pip install -r requirements.txt
jupyter notebook "MNIST_Digit_Classification_CNN VS ANN.ipynb"

