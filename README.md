# Customer Analytics: Experimentation and Uplift Testing

## 📌 Project Overview

This project demonstrates how to perform **experimentation and uplift testing** using customer transaction data. The goal is to evaluate the impact of marketing trials (run in selected stores) by comparing them with control stores that have similar pre-trial performance.

We use statistical and visualization techniques to:

* Summarize store-level performance over time.
* Select control stores for each trial store using correlation.
* Compare trial vs control stores during the experiment period.
* Visualize differences in sales, customer count, and transactions per customer.

---

## 📂 Dataset

The notebook expects an input dataset named **`QVI_data.csv`**, which includes transaction-level details:

* `STORE_NBR` – Store number
* `DATE` – Transaction date
* `TOT_SALES` – Total sales value
* `LYLTY_CARD_NBR` – Unique customer card number
* `TXN_ID` – Transaction ID

---

## ⚙️ Workflow

1. **Data Preparation**

   * Load and clean dataset.
   * Convert dates and create monthly summaries.

2. **Monthly Store Summaries**

   * Compute key metrics: total sales, number of customers, number of transactions, and transactions per customer.

3. **Trial & Control Store Selection**

   * Define trial stores (77, 86, 88).
   * Use correlation of pre-trial sales trends to select the most similar control store for each trial store.

4. **Performance Comparison**

   * Compare sales, customer count, and transactions during trial months vs control stores.

5. **Visualization**

   * Generate plots showing trial vs control store performance.
   * Highlight the trial period for easy interpretation.

---

## 🛠️ Technologies Used

* **Python 3**
* **Pandas** – data manipulation
* **NumPy** – numerical calculations
* **Matplotlib** – visualizations

---

## 📊 Key Insights

* Identifies which stores are best matched as controls for trials.
* Measures uplift in sales and customer engagement during trial.
* Provides clear visual evidence of trial impact vs natural variation.

---

## 🚀 How to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/customer-analytics-experimentation.git
   ```
2. Navigate to the project folder:

   ```bash
   cd customer-analytics-experimentation
   ```
3. Open the Jupyter Notebook:

   ```bash
   jupyter notebook Customer_Analytics_Experimentation_and_Uplift_testing.ipynb
   ```
4. Ensure `QVI_data.csv` is in the same folder.
5. Run cells step by step to reproduce results and plots.

---

## 📈 Example Output

* Monthly sales summary tables.
* Trial vs control comparison statistics.
* Plots of **Sales**, **Customers**, and **Transactions per Customer** for trial vs control stores.

---

## 📌 Author

Developed by **Suhas G R** as part of a customer analytics experimentation study.

---

## 🔑 Keywords

Customer Analytics, Uplift Testing, Experimentation, A/B Testing, Control Store, Retail Analytics, Python, Pandas, Matplotlib
