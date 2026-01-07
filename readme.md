# Customer Segmentation using K-Means Clustering

This project applies K-Means clustering to segment retail customers based on their purchasing behavior. The goal is to help businesses understand different customer types and apply targeted marketing strategies.

---

## 📌 Problem Statement
Retail stores serve customers with very different spending behaviors. Treating all customers the same leads to inefficient marketing and lost revenue.  
This project groups customers into meaningful segments using unsupervised machine learning.

---

## 📂 Dataset
The project uses the **Mall Customers Dataset** from Kaggle.

Each customer has:
- Gender
- Age
- Annual Income
- Spending Score

---

## 🎯 Features Used for Clustering
For meaningful segmentation, only behavioral and financial features were used:
- **Annual Income**
- **Spending Score**

CustomerID and Gender were excluded because they do not represent purchasing behavior.

---

## 🛠️ Methodology

1. Data loading and cleaning  
2. Exploratory Data Analysis (EDA)  
3. Feature selection  
4. Feature scaling using **StandardScaler**  
5. Optimal cluster selection using:
   - Elbow Method  
   - Silhouette Score  
6. K-Means clustering  
7. Business interpretation of clusters  

---

## 📊 Model Performance

The Silhouette Score was used to evaluate clustering quality.  
The model achieved a **strong score**, indicating well-separated and meaningful customer groups.

---

## 🧩 Customer Segments Identified

The model grouped customers into 5 clusters:

- **VIP Customers** – High income, high spending  
- **Wealthy but Frugal** – High income, low spending  
- **Discount Lovers** – Low income, high spending  
- **Low Value Customers** – Low income, low spending  
- **Stable Middle Class** – Medium income and spending  

These segments can be used for targeted marketing, promotions, and customer retention strategies.

---

## 📁 Files in this Repository

- `customer_segmentation.ipynb` – Full analysis and training notebook  
- `train.py` – Reproducible training script  
- `kmeans_model.pkl` – Trained K-Means model  
- `scaler.pkl` – Feature scaler  
- `clustered_customers.csv` – Dataset with assigned clusters  
- `Mall_Customers.csv` – Original dataset  
- `requirements.txt` – Required Python libraries  

---

## 🚀 How to Run

Install dependencies:
```bash
pip install -r requirements.txt
