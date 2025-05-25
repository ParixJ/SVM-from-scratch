# 🌸 SVM from Scratch – Iris Dataset Classification

This project implements a **Support Vector Machine (SVM)** from scratch (without using `sklearn.svm.SVC`) to classify **Setosa** and **Virginica** species from the famous **Iris dataset**.

## 📝 Features
✅ Implements **linear SVM** with hinge loss and L2 regularization  
✅ Gradient-based **stochastic gradient descent (SGD)** training  
✅ **Visualization** of dataset  
✅ No external SVM libraries – implemented from scratch using `NumPy`  

## 🚀 How It Works
1️⃣ **Dataset**: Loads the first 100 samples (Setosa and Virginica) from the Iris dataset.  
2️⃣ **Label Mapping**: Converts labels to \{-1, 1\}.  
3️⃣ **Model**: Initializes weights and bias, computes hinge loss and gradients.  
4️⃣ **Training**: Uses SGD to optimize weights and bias.  
5️⃣ **Visualization**: Plots the data points.
6️⃣ **Loss**: Combines hinge loss and L2 regularization.

## 📊 Results
- **Separates** Setosa and Virginica using a linear decision boundary.
- **Loss function** optimised using gradient descent:
```python
x2 = -(w[2]/w[3]) * x1 - (b/w[3])  # using features 2 and 3
