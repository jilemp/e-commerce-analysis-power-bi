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
📂 Ecommerce-Analysis-PowerBI/
├── 📊 Ecommerce_Analysis.pbix
├── 📝 README.md
├── 📁 Data/
│   └── sample_data.csv (or provided source files)
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

✅ Project Status
✅ Completed
🧠 Skills Applied: Power Query, DAX, Data Modeling, Report Design
📅 Duration: ~4 hours

📄 License
This project is a case study based on DataCamp content and intended for educational and portfolio purposes only.

🙋‍♂️ Author
Your Name
GitHub: @yourusername
LinkedIn: Your LinkedIn Profile

yaml
Copy
Edit

---

### ✅ Next Steps

If you want, I can:
- Help you generate preview screenshots
- Write up a `/DAX/key_measures.md` file
- Guide you on creating a GitHub Page for it

Let me know how you'd like to proceed!





You said:
please put everything in an exportable .md file


ChatGPT said:
Sure! Here's the entire README.md file packaged in Markdown format. You can copy the text below and save it as a .md file using any text editor (like Notepad, VS Code, or directly in GitHub when creating a new file).

📄 Download-ready README.md file content:

markdown
Copy
Edit
# 📊 Ecommerce Analysis in Power BI

A complete Power BI case study analyzing an online pet supply store called **Whiskique**. This project explores sales and shipping performance across regions, products, and customer segments, using advanced data modeling, Power Query transformations, and DAX measures.

---

## 🧠 Project Overview

Case Study: Ecommerce Analysis in Power BI**. It simulates a real-world business scenario where data-driven insights are used to support strategic decisions for an ecommerce company.

Through data modeling, transformation, analytics, and visualization, this dashboard helps answer key business questions:

- How are sales and expenses distributed across regions?
- Which products and customers are most profitable?
- What are the key drivers of shipping costs?
- How can we optimize operations based on a what-if scenario?

---

## 📁 Project Structure

```bash
📂 Ecommerce-Analysis-PowerBI/
├── 📊 Ecommerce_Analysis.pbix
├── 📝 README.md
├── 📁 Data/
│   └── sample_data.csv (or provided source files)
├── 📁 Images/
│   └── dashboard_preview.png
├── 📁 DAX/
│   └── key_measures.md
```

---

## 🧾 Key Features

### 🔍 1. **Data Exploration**
- Combined multiple datasets to create a clean model.
- Applied Power Query for filtering, cleaning, and transformation.
- Built metrics for orders, customers, and purchases.
- Identified commonly purchased product pairs.

### 📈 2. **Ecommerce Analytics**
- Created DAX measures for:
  - Profitability by product and customer
  - Sales by state and region
  - Shipping cost metrics
- Implemented a **What-If Analysis** to evaluate bulk shipping strategies.

### 📊 3. **Visualize Your Analysis**
- Created dashboard-style reports including:
  - **Revenue & Profit Trends**
  - **Executive Summary**
  - **Shipping Cost Dashboard**
  - **Profit Percentage Treemap**
- Developed a final cohesive story with actionable insights.

---

## 📸 Report Screenshots

![Dashboard Preview](Images/dashboard_preview.png)

---

## 📌 Tools & Technologies
- **Power BI Desktop**
- **Power Query (M language)**
- **DAX (Data Analysis Expressions)**
- Sample datasets from **DataCamp Sandbox**

---

## 🧮 Sample DAX Measures

```DAX
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
```

> Full DAX measures available in `/DAX/key_measures.md`

---

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
