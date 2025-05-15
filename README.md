
# 🧠 Customer Segmentation with SQL & Tableau

## 📘 Project Overview
This project showcases a classic **RFM analysis** (Recency, Frequency, Monetary) using **SQL (MySQL)** and **Tableau** to segment customers based on purchase behavior and demographics.

We start with raw transactional data, normalize it into separate `customers` and `orders` tables, calculate RFM scores, and visualize insights with a professional dashboard.

---

## 🛠️ Tools Used

- **MySQL Workbench** – Data manipulation & RFM scoring
- **SQL** – Aggregations, CTEs, scoring logic
- **Tableau Desktop** – Dashboard design and interactivity
- **GitHub** – Version control and portfolio hosting

---

## 🧮 Data Modeling

Data was split into two normalized tables:

### `customers` table:
| CustomerID | Gender | Age | Country |
|------------|--------|-----|---------|

### `orders` table:
| OrderID | CustomerID | OrderDate | OrderAmount |
|---------|------------|-----------|-------------|

An RFM view (`rfm_metrics`) was created in MySQL for direct Tableau consumption.

---

## 📊 Dashboard Features

### ✅ KPIs
- **Average Order Amount**
- **Total Customers**
- **Top 5 Countries by Customer Count**

### 📈 Charts
- **Bar Chart**: Count of customers by RFM Segment
- **Heat Map**: R x F grid, colored by Monetary score

### 🎛️ Filters
- Gender
- Country
- Age Group (Calculated in Tableau)

---

## 🧠 Key Insights

- Top-spending customer segments tend to be younger and concentrated in fewer countries.
- Customers with recent, frequent purchases are high-value, even if individual orders are smaller.
- Demographics (Gender & Age) have strong correlation with RFM profiles in some regions.

---

## 📁 Repo Structure

```
customer-segmentation-sql-tableau/
│
├── data/
│   ├── customers.csv
│   └── orders.csv
│
├── sql/
│   └── create_rfm_view.sql
│
├── tableau/
│   └── dashboard_design.twb (optional)
│
├── README.md
└── LICENSE
```

---

## 📝 Next Steps

- Add clustering or classification model on top of RFM
- Automate data pipeline refresh
- Embed Tableau dashboard online for recruiters

---

## 📬 Connect

Feel free to fork this repo and make it your own. Questions or ideas? Reach out!

---
