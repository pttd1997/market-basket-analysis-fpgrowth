# 🧺 Market Basket Analysis Using FP-Growth (Databricks + PySpark)

This project performs Market Basket Analysis on a retail transactions dataset using the FP-Growth algorithm in PySpark, within the Databricks platform.

## 🚀 Objective
Uncover frequent itemsets and association rules from customer transaction data to support strategic business decisions such as product placement and bundling.

## 📂 Dataset
- Format: CSV
- Source: Groceries dataset
- Description: Each row contains a unique customer transaction listing purchased items.

## 🔧 Tools & Technologies
- Python
- PySpark
- Databricks (Community Edition)
- FP-Growth (MLlib)
- Spark SQL

## 🧠 Methodology
1. Data loaded and preprocessed in Spark.
2. Transactions grouped and nulls removed.
3. FP-Growth algorithm applied to detect frequent itemsets and generate association rules.
4. Rules sorted by confidence for business relevance.

## 📊 Visualizations

### 🔄 Chord Diagram of Association Rules

<img width="741" alt="Chord Diagram" src="https://github.com/user-attachments/assets/8693e40e-c2d3-4ff8-8a49-7f970d869933" />

This visualization displays the relationships between items in the form of directional association rules.  
- **Blue arrows** represent outgoing rules: `Antecedent → Consequent`  
- **Red arrows** show incoming rules: `Consequent → Antecedent`  
It helps identify central items influencing many other purchases.

---

### 📈 Frequent Itemsets & Top Association Rules

<img width="741" alt="Frequent Itemsets and Top Rules" src="https://github.com/user-attachments/assets/22f5f40a-1e25-48fd-b3d4-21c648f50a87" />

- **Bar Chart**: Top 10 most frequently purchased items across all transactions.
- **Pie Chart**: Top 10 association rules ranked by **Lift**, showing strong co-occurrence patterns like:
  - `{rolls/buns, other vegetables} → {whole milk}`
  - `{sausage, rolls/buns} → {whole milk}`

These insights support potential strategies for cross-selling and product bundling.

