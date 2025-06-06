# 📊 Ecommerce Analysis in Power BI

A complete Power BI case study analyzing an online pet supply store called **Whiskique**. This project explores sales and shipping performance across regions, products, and customer segments, using advanced data modeling, Power Query transformations, and DAX measures.

---

## 🧠 Project Overview

This project is part of the **DataCamp Case Study: Ecommerce Analysis in Power BI**. It simulates a real-world business scenario where data-driven insights are used to support strategic decisions for an ecommerce company.

Through data modeling, transformation, analytics, and visualization, this dashboard helps answer key business questions:

- How are sales and expenses distributed across regions?
- Which products and customers are most profitable?
- What are the key drivers of shipping costs?
- How can we optimize operations based on a what-if scenario?

---

## 📁 Project Structure

```bash
📂 e-commerce-analysis-power-bi/
├── 📊 e-commerce_analysis.pbix
├── 📝 README.md
├── 📁 datasets/
│   └── dim_customers.csv
│   └── dim_products.csv
│   └── fact_sales.csv
│   └── state_region_mapping.csv
├── 📁 Images/
│   └── dashboard_preview.png
├── 📁 DAX/
│   └── key_measures.md
🧾 Key Features
🔍 1. Data Exploration
Combined multiple datasets to create a clean model.

Applied Power Query for filtering, cleaning, and transformation.

Built metrics for orders, customers, and purchases.

Identified commonly purchased product pairs.

📈 2. Ecommerce Analytics
Created DAX measures for:

Profitability by product and customer

Sales by state and region

Shipping cost metrics

Implemented a What-If Analysis to evaluate bulk shipping strategies.

📊 3. Visualize Your Analysis
Created dashboard-style reports including:

Revenue & Profit Trends

Executive Summary

Shipping Cost Dashboard

Profit Percentage Treemap

Developed a final cohesive story with actionable insights.

📸 Report Screenshots
Add screenshots to the Images/ folder and embed them below:


📌 Tools & Technologies
Power BI Desktop

Power Query (M language)

DAX (Data Analysis Expressions)

Sample datasets from DataCamp Sandbox

🧮 Sample DAX Measures
DAX
Copy
Edit
Total Sales = SUM(Sales[SalesAmount])

Profit Margin % = 
DIVIDE(
    [Total Profit],
    [Total Sales],
    0
)

Sales by State = 
CALCULATE(
    [Total Sales],
    ALLEXCEPT(Customer, Customer[State])
)
Full DAX measures available in /DAX/key_measures.md

## ✅ Project Status

✅ Completed  
🧠 Skills Applied: Power Query, DAX, Data Modeling, Report Design  
📅 Duration: ~4 hours

---

## 📄 License

This project is a case study based on DataCamp content and intended for **educational and portfolio** purposes only.

---

## 🙋‍♂️ Author

**Your Name**  
GitHub: [@jilemp](https://github.com/jilemp)  
LinkedIn: [Jose Ignacio Ibarra Lemp](https://linkedin.com/in/jose-ignacio-ibarra)
