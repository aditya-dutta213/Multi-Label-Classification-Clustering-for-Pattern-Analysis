### **Multi-Label Classification & Clustering for Pattern Analysis**  
**Author:** Aditya Dutta  
**Date:** Oct 2024 - Nov 2024  
**Technologies:** Python, Scikit-Learn, SMOTE, SVMs, K-Means  

---

## **Project Overview**  
This project explores **multi-label classification and clustering** using the **Anuran Calls (MFCCs) dataset**. The dataset contains **frog call recordings** classified into multiple hierarchical categories: **Family, Genus, and Species**. The project employs **Support Vector Machines (SVMs) with Gaussian kernels** for classification and **K-Means clustering with Monte Carlo simulations** for pattern discovery.

---

## **Dataset**  
The dataset is sourced from the **Anuran Calls (MFCCs) dataset** available at:  
🔗 [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Anuran+Calls+%28MFCCs%29)  

- **7,195 samples** of frog call recordings  
- **22 MFCC (Mel-Frequency Cepstral Coefficient) features**  
- **Three hierarchical labels:**  
  - **Family** (4 categories)  
  - **Genus** (8 categories)  
  - **Species** (10 categories)  
- **Objective:** Perform multi-label classification & cluster analysis  

---

## **Methods & Techniques**  

### **1. Multi-Label Classification**  
✔ **Data Preprocessing** – Standardized MFCC features using **Scikit-Learn**  
✔ **Exact Match & Hamming Loss Metrics** – Evaluated classifier performance  
✔ **Support Vector Machines (SVMs)** – One-vs-All SVMs trained per label  
✔ **Hyperparameter Tuning** – Optimized SVM kernel and C-penalty using **10-fold cross-validation**  
✔ **SMOTE Oversampling** – Addressed class imbalance in labels  

### **2. Clustering Analysis**  
📌 **K-Means Clustering** – Grouped species using feature similarities  
📌 **Monte Carlo Simulations** – Performed **50 iterations** to validate cluster consistency  
📌 **Silhouette Score Analysis** – Measured clustering quality  

---

## **Results & Findings**  

| Model                 | Accuracy | F1-Score (Family) | F1-Score (Genus) | F1-Score (Species) |  
|----------------------|------------|----------------|----------------|----------------|  
| SVM (Without SMOTE)  | **96.8%**  | **0.88**  | **0.96**  | **0.94**  |  
| **SVM + SMOTE** ✅ | **98.9%**  | **0.99**  | **0.98**  | **0.96**  |  
| K-Means Clustering | **-**  | **-**  | **-**  | **Silhouette Score: 0.85** |  

✔ **SMOTE significantly improved minority class recognition**  
✔ **SVM with Gaussian kernel delivered the best classification results**  
✔ **K-Means clustering revealed strong species-specific acoustic patterns**  

---

## **How to Run the Project**  
1️⃣ Install dependencies:  
```bash
pip install pandas numpy scikit-learn imbalanced-learn matplotlib seaborn
```
2️⃣ Download the dataset from [UCI ML Repository](https://archive.ics.uci.edu/ml/datasets/Anuran+Calls+%28MFCCs%29)  
3️⃣ Run the **Jupyter Notebook** or execute the script:  
```bash
python multi_label_classification.py
```

---

## **Key Takeaways**  
🔹 **Multi-label classification requires specialized metrics** (Exact Match, Hamming Loss)  
🔹 **SVM with Gaussian kernel performed best with cross-validation tuning**  
🔹 **SMOTE significantly enhanced minority class prediction**  
🔹 **Clustering analysis can reveal species-specific patterns in bioacoustic data**  

---

## **Future Improvements**  
🚀 **Explore Deep Learning models (CNNs, RNNs) for audio feature extraction**  
🚀 **Implement Hierarchical Classification to account for label relationships**  
🚀 **Use DBSCAN or Spectral Clustering for better pattern recognition**  

---

### 📌 **Contact**  
For any questions or improvements, feel free to connect! 🚀  

