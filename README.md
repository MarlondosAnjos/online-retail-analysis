# Online Retail II — Sales & Customer Analysis

🌐 **Languages:** English | [Português (Brasil)](README.pt-BR.md)

## Project Overview

This project presents an exploratory data analysis of the **Online Retail II** dataset, covering transactions from December 2009 to December 2011.

The goal is to evaluate retail business performance through sales trends, product demand, customer purchasing behavior, and revenue concentration. The analysis also considers cancellations to distinguish Gross Sales from Net Sales and provide a more accurate view of recorded revenue.

The project uses Python, Pandas, and Matplotlib to transform transaction-level data into actionable business insights.

## Business Questions

1. How did sales performance evolve over time?
2. Which products generated the highest revenue and sales volume?
3. Who were the highest-value customers, and how did their purchasing behaviors differ?
4. Which products were most frequently purchased by high-value customers?
5. How concentrated was revenue among high-value customers, and how much did these customers contribute to best-selling products?

## Key Findings

### Overall Business Performance

- **Gross Sales:** approximately **£20.47 million**.
- **Cancellation Value:** approximately **£1.46 million**.
- **Net Sales:** approximately **£19.00 million**.

Accounting for cancellations provides a more accurate measure of recorded revenue than Gross Sales alone.

### Product Performance

- **REGENCY CAKESTAND 3 TIER** generated the highest Net Sales, approximately **£314,045**.
- **WORLD WAR 2 GLIDERS ASSTD DESIGNS** led in net units sold, with **104,435 units**.
- None of the Top 10 products by net units sold appeared among the Top 10 products by cancelled units.
- Two products appeared in both the Top 10 by Net Sales and the Top 10 by cancellation value. Their cancellation values represented approximately **5.00%** and **3.64%** of their respective Gross Sales.

These findings demonstrate why revenue, sales volume, and cancellations should be evaluated together rather than in isolation.

### Customer Behavior

- **Customer 18102** was the highest-value customer, generating approximately **£570,381** in Net Spending.
- Among the Top 10 highest-value customers, **REGENCY CAKESTAND 3 TIER** appeared in **199 distinct invoices**.
- **PACK OF 72 RETROSPOT CAKE CASES** led in net units purchased by these customers, with **20,376 units**.

Purchasing frequency and unit volume provide different perspectives on customer preferences.

### Revenue Concentration

- The Top 10 highest-value customers generated approximately **£2.66 million**, representing **13.97%** of total Net Sales.
- These customers contributed **17.61%** of REGENCY CAKESTAND 3 TIER's Net Sales, compared with **3.59%** of CHILLI LIGHTS' Net Sales.

This highlights the importance of high-value customers while showing that their influence varies considerably across products.

## Data Visualizations

### Top 10 Products by Net Sales

![Top 10 Products by Net Sales](images/top_10_products_net_sales.png)

**Business insight:** REGENCY CAKESTAND 3 TIER generated the highest Net Sales, at approximately £314,045. This highlights the importance of evaluating product performance by revenue, not only by units sold.

### Revenue Concentration — Top 10 Customers

![Revenue Concentration — Top 10 Customers](images/top_10_customers_revenue_concentration.png)

**Business insight:** The Top 10 highest-value customers contributed £2.66 million, representing 13.97% of total Net Sales. The remaining 86.03% came from other transactions, including those without a Customer ID. This highlights the importance of high-value customers while providing context for their contribution to overall revenue.

## Business Recommendations

- Strengthen retention initiatives for high-value customers.
- Consider both revenue and unit demand when planning inventory.
- Tailor product marketing to purchasing frequency and customer preferences.
- Monitor revenue concentration to understand dependence on high-value customers.
- Evaluate cancellations alongside sales and investigate unusually large cancellation transactions separately.

## Tools and Technologies

- **Python** — data analysis
- **Pandas** — data cleaning, transformation, and aggregation
- **Matplotlib** — data visualization
- **Jupyter Notebook** — exploratory analysis and documentation
- **Visual Studio Code** — development environment

## Project Structure

```text
online-retail-analysis/
├── data/
│   └── raw/
│       └── online_retail_II.xlsx
├── notebooks/
│   └── online_retail_analysis.ipynb
├── README.md
└── .gitignore
```

## How to Run the Project

**Python version:** Developed and tested with Python 3.14.3.

1. Clone or download this repository.
2. Install Python and the required libraries:

   ```bash
   pip install pandas matplotlib openpyxl notebook
   ```

3. Open `notebooks/online_retail_analysis.ipynb` in VS Code or Jupyter Notebook.
4. Run the notebook cells in order.

The dataset is stored in `data/raw/`, and the notebook accesses it through a relative file path.

## Dataset Source and Attribution

**Dataset:** Online Retail II  
**Creator:** Daqing Chen  
**Repository:** UCI Machine Learning Repository  
**Source:** https://archive.ics.uci.edu/dataset/502/online+retail+ii  
**DOI:** https://doi.org/10.24432/C5CG6D  
**License:** Creative Commons Attribution 4.0 International (CC BY 4.0)

The dataset is used for educational and portfolio purposes, with attribution to its original creator and repository.