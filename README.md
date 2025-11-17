
# 🧠 Dimensionality Reduction on MNIST  
### PCA • t-SNE • Random Forest • SGDClassifier  
This project focuses on applying dimensionality reduction techniques to the MNIST handwritten digits dataset and comparing classifier performance before and after reducing the number of features.

It contains the completed solution for **Questions 9 and 10** of a Machine Learning assignment using PCA and t-SNE.

---

## 📌 Project Overview

This notebook explores:

### **1️⃣ Training ML models on the full MNIST dataset (784 features)**
- Random Forest Classifier  
- SGD Classifier  

### **2️⃣ Reducing dimensionality using PCA (95% explained variance)**
- Finds the minimum number of components needed to retain 95% of the variance  
- Retrains both classifiers on compressed data  
- Compares training time and accuracy  

### **3️⃣ Visualizing MNIST in 2D**
Using **t-SNE**, and optionally:
- PCA (2D)
- LLE
- MDS

This provides intuitive visual clusters for digits 0–9.

---

## 📊 Key Results Summary

### **💻 Random Forest**
| Model | Training Time | Test Accuracy |
|-------|----------------|----------------|
| RF (Original 784 dims) | ~X sec | ~X% |
| RF (PCA-Reduced) | ~X sec | ~X% |

➡️ Typically, PCA **reduces training time** but accuracy may slightly change.

---

### **⚡ SGDClassifier**
| Model | Training Time | Test Accuracy |
|-------|----------------|----------------|
| SGD (Original) | ~X sec | ~X% |
| SGD (PCA-Reduced) | ~X sec | ~X% |

➡️ SGD often benefits **more** from PCA because it speeds up gradient updates.

---

### **🌀 t-SNE 2D Visualization**
- Clusters for digits 0–9 appear with strong separation  
- Outliers show overlapping classes (e.g., 4 vs. 9)

This helps understand class structure and dataset geometry.

---

## 📁 Files Included
```
📦 Dimensionality-Reduction-MNIST
 ┣ 📄 dimensionality_reduction_mnist.ipynb
 ┣ 📄 README.md
 ┗ 📁 (Optional) images/ - t-SNE, PCA, LLE, MDS visualizations
```

---

## 🚀 How to Run
1. Clone the repo:
```bash
git clone https://github.com/yourusername/Dimensionality-Reduction-MNIST.git
```

2. Install dependencies:
```bash
pip install numpy matplotlib scikit-learn
```

3. Launch the notebook:
```bash
jupyter notebook dimensionality_reduction_mnist.ipynb
```

---

## 🧠 What You Learn From This Project
- How PCA reduces noise & speeds up training  
- How to compare model performance across different input spaces  
- How t-SNE reveals meaningful structure in high-dimensional data  
- How dimensionality impacts machine learning workflows  

---

## ⭐ Future Improvements
- Try UMAP for faster nonlinear reduction  
- Add Autoencoders for deep learning–based compression  
- Compare different PCA variance thresholds (90%, 99%)  

