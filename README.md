# 📊 Customer Segmentation and Churn Prediction

## 📌 Project Overview

This project performs **customer segmentation and churn prediction** using transaction data.

The project uses **RFM Analysis** to understand customer behavior, **K-Means Clustering** to create customer segments, and **Logistic Regression** to predict customer churn.

---

## 🎯 Objectives

* Analyze customer purchasing behavior
* Calculate **RFM (Recency, Frequency, Monetary)** features
* Segment customers using **K-Means Clustering**
* Identify different types of customers
* Predict customer churn using **Logistic Regression**
* Visualize customer segments and model results

---

## 📂 Dataset

The project uses the `OnlineRetail_clean.csv` dataset.

The dataset contains online retail transaction information used to calculate customer-level RFM metrics.

---

## 🛠️ Technologies Used

* 🐍 Python
* 🐼 Pandas
* 🔢 NumPy
* 📈 Matplotlib
* 📊 Seaborn
* 🤖 Scikit-learn
* ☁️ Google Colab
* 📓 Jupyter Notebook

---

## 🔄 Project Workflow

### 1️⃣ Data Loading

The dataset is loaded using **Pandas**.

### 2️⃣ Data Cleaning

* Remove missing `CustomerID` values
* Convert `InvoiceDate` into datetime format
* Calculate `TotalPrice` using:

```python
TotalPrice = Quantity * UnitPrice
```

### 3️⃣ 📊 RFM Analysis

Three important customer features are calculated:

* **Recency** → Number of days since the customer's most recent purchase
* **Frequency** → Number of unique invoices/orders made by the customer
* **Monetary** → Total amount spent by the customer

### 4️⃣ ⚖️ Feature Scaling

`StandardScaler` is used to scale the RFM features before clustering.

### 5️⃣ 👥 Customer Segmentation

**K-Means Clustering** is used to divide customers into **4 clusters**.

### 6️⃣ 🚨 Churn Prediction

A churn label is created based on customer Recency.

Customers with **Recency greater than 90 days** are classified as churned customers.

**Logistic Regression** is then used to predict customer churn.

### 7️⃣ 📈 Model Evaluation

The Logistic Regression model is evaluated using:

* Classification Report
* Accuracy Score
* Confusion Matrix

### 8️⃣ 📊 Visualization

The project includes several visualizations:

* Customer Segmentation
* Elbow Method
* Cluster Analysis
* Frequency vs Monetary
* Cluster vs Monetary
* Recency Distribution
* Frequency Distribution
* Monetary Distribution
* Customer Segment Count
* Customer Type Distribution
* Confusion Matrix

---

## 👥 Customer Segments

The project assigns customer types based on their clusters:

* ⭐ **Loyal Customers**
* 🆕 **New Customers**
* 💡 **Potential Customers**
* ⚠️ **At Risk Customers**

---

## 📁 Project Files

```text
Customer-Segmentation/
│
├── 📓 Customer_Segmentation_Project.ipynb
├── 🐍 customer_segmentation_project.py
├── 📊 OnlineRetail_clean.csv
├── 📄 Final_Customer_Segmentation.csv
├── 📖 README.md
├── 📦 requirements.txt
└── 🚫 .gitignore
```

---

## ▶️ How to Run

### ☁️ Using Google Colab

1. Open `Customer_Segmentation_Project.ipynb`
2. Upload `OnlineRetail_clean.csv`
3. Run all cells
4. The analysis, visualizations and model results will be generated
5. The final customer segmentation data will be saved as `Final_Customer_Segmentation.csv`

### 💻 Using Local Python

Install the required libraries:

```bash
pip install -r requirements.txt
```

Then run:

```bash
python customer_segmentation_project.py
```

---

## 📤 Output

The project generates:

```text
Final_Customer_Segmentation.csv
```

This file contains the customer-level segmentation results and related features.

---

## 🧠 Machine Learning Models

### K-Means Clustering

Used for **customer segmentation** based on RFM features.

### Logistic Regression

Used for **customer churn prediction**.

---

## 📌 Conclusion

This project demonstrates how customer transaction data can be transformed into meaningful customer segments using **RFM Analysis** and **K-Means Clustering**.

**Logistic Regression** is also used to predict customer churn based on customer-level RFM features.

The analysis can help businesses:

* Understand customer behavior
* Identify valuable customers
* Identify potential customers
* Identify customers who may be at risk of churn
* Support customer retention strategies

---

📌 Data Science Project
🐍 Python | Machine Learning | Customer Analytics
