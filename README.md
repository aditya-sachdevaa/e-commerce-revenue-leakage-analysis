# e-commerce-revenue-leakage-analysis
Analysis of an e-commerce dataset to detect and quantify revenue leakage from cancellations, returns, and irregular pricing.
# 📦 E-commerce Revenue Leakage Analysis

## 📌 Project Overview
This project analyzes transaction data from a UK-based online retailer to identify potential revenue leakage points. The dataset covers purchases made between 2010 and 2011, including canceled orders, returns, and irregular pricing.

**Objectives:**
- Detect and quantify revenue losses from cancellations, returns, and low pricing.
- Provide actionable insights to reduce leakage and improve profitability.

---

## 🗂 Dataset
- **Source:** [E- Commerce Data](https://www.kaggle.com/datasets/carrie1/ecommerce-data)
- **Rows:** ~500,000 transactions  
- **Features:** InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country  
- *(Note: Dataset is not included in this repository due to size/licensing — link above can be used to download.)*

---

## 🔍 Key Steps in Analysis
1. **Data Cleaning**
   - Removed null values in `CustomerID`
   - Dropped canceled transactions (`InvoiceNo` starting with "C")
   - Removed duplicate entries
   - Dropped irrelevant "Manual" rows

2. **Exploratory Data Analysis**
   - Seasonal trends in sales
   - High-value customer analysis
   - Detection of irregular pricing patterns

3. **Insights**
   - Cancellations and returns contribute significantly to revenue loss.
   - Certain products repeatedly show higher return rates.

---

## 📊 Sample Visualizations 
**Seasonal Trends**<img width="1210" height="599" alt="image" src="https://github.com/user-attachments/assets/b3b90e21-f1e3-4675-8861-c1ae12e9d568" />

**Effects of Cancelations**<img width="1214" height="574" alt="image" src="https://github.com/user-attachments/assets/217dd40a-072f-4a66-9b94-2260b5b2c580" />


---

## 🛠 Tech Stack
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 🚀 How to Run the Project

```bash
# 1. Clone the repository
git clone https://github.com/aditya-sachdevaa/e-commerce-revenue-leakage-analysis.git

# 2. Navigate to the project folder
cd e-commerce-revenue-leakage-analysis

# 3. Install required libraries
pip install pandas numpy matplotlib seaborn jupyter

# 4. Download the dataset from UCI Machine Learning Repository
#    https://archive.ics.uci.edu/ml/datasets/online+retail
#    and place it in the project folder

# 5. Open the Jupyter Notebook
jupyter notebook E-Comm_RevenueLeakage_Analysis.ipynb

