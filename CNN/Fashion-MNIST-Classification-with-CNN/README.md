# 👗 Fashion MNIST Classification with CNN

## 📌 Overview  
This project implements a **Convolutional Neural Network (CNN)** to classify images from the **Fashion MNIST dataset**.  
The dataset contains 10 categories of clothing items (e.g., T-shirt, Trouser, Dress, Coat, etc.), each represented as a 28×28 grayscale image.  

The goal is to build a CNN model that achieves high accuracy on this real-world image classification task.

---

## 🗂️ Dataset  
- **Source**:Keras Library
- **Samples**: 60,000 for training + 10,000 for testing  
- **Classes**: 10 fashion categories  
- **Image format**: 28×28 grayscale  
- **Preprocessing**:  
  - Normalization to [0, 1]  
  - Reshaping to `(28, 28, 1)` to fit CNN input  

---

## ⚙️ Model Architecture (CNN)  
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
- **Epochs**: 15  
- **Batch size**: 64  
- **Early Stopping**: Used to prevent overfitting  

---

## 📊 Results (Summary)  
> Results may vary depending on hardware and number of epochs.

- Achieved **~92–93% accuracy** on the test set.  
- Training and validation curves (Loss & Accuracy) show good convergence.  

---

## 🚀 How to Run  
```bash
git clone <repo-url>
cd <repo-name>
pip install -r requirements.txt
jupyter notebook "Fashion_MNIST_Digit_Classification_CNN.ipynb"

