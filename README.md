

# 📊 Blinkit Data Analysis Project

![Blinkit data analysis_page-0001](https://github.com/user-attachments/assets/f5464490-1f51-4b35-993b-ea4d7f1a349e)


## 📌 Case Study

Blinkit is one of India’s leading quick-commerce grocery delivery companies.
This project analyzes **sales, product categories, outlet performance, and customer preferences** to generate actionable insights.

**Objective:**

* Identify factors influencing sales
* Provide recommendations to improve revenue, customer satisfaction, and outlet efficiency

---

## 🗄️ Database Description

The dataset **`BlinkIT Grocery Data.xlsx`** consists of transactional and categorical information about grocery items sold across different outlets.

### **Table: Grocery Sales Data**

| Column Name                   | Description                                                           |
| ----------------------------- | --------------------------------------------------------------------- |
| **Item Identifier**           | Unique product code for each grocery item                             |
| **Item Fat Content**          | Type of fat content (Low Fat, Regular, etc.)                          |
| **Item Type**                 | Category of product (Fruits, Frozen Foods, Canned, Soft Drinks, etc.) |
| **Item Weight**               | Weight of the item in kilograms                                       |
| **Item Visibility**           | Proportion of display area allocated to the item in the store         |
| **Outlet Identifier**         | Unique ID for each store                                              |
| **Outlet Establishment Year** | Year when the outlet was established                                  |
| **Outlet Location Type**      | Tier of the outlet location (Tier 1, Tier 2, Tier 3)                  |
| **Outlet Size**               | Size of the outlet (Small, Medium, High)                              |
| **Outlet Type**               | Type of supermarket (Supermarket Type1, Type2, Type3, Grocery Store)  |
| **Sales**                     | Total sales value of the product                                      |
| **Rating**                    | Customer rating for the product (scale of 1–5)                        |

---

## 🧹 Data Cleaning

* ✅ Handled **missing values** in `Item Weight` and `Sales`
* ✅ Standardized **categorical fields** (e.g., `LF`, `low fat` → `Low Fat`)
* ✅ Treated **outliers** in `Item Visibility` and `Sales`
* ✅ Encoded categorical variables for analysis

---

## 📈 Data Analysis & Insights

**Dataset Summary:**

* 📌 Total Records: **8,523**
* 📦 Unique Items: **1,559**
* 🏬 Unique Outlets: **10**
* 💰 Total Sales: **₹1.2M**
* 📉 Average Sales per Item: **₹141**


---

## 🧮 Measures & DAX Formulas

The following **DAX measures** were created in Power BI for analysis:

```DAX
-- Total Sales
Total Sales = SUM('BlinkIT Grocery Data'[Sales])

-- Average Sales
Average Sales = AVERAGE('BlinkIT Grocery Data'[Sales])


-- Average Rating
Average Rating = AVERAGE('BlinkIT Grocery Data'[Rating])

-- No. of Items
No. of Items = COUNTROWS('BlinkIT Grocery Data')


-- Metrics = {
    ("Total Sales", NAMEOF('BlinkIT Grocery Data'[Total Sales]), 0),
    ("Avg Sales", NAMEOF('BlinkIT Grocery Data'[Avg Sales]), 1),
    ("No. of Items", NAMEOF('BlinkIT Grocery Data'[No. of Items]), 2),
    ("Avg Rating", NAMEOF('BlinkIT Grocery Data'[Avg Rating]), 3)
}
```

---

## 🚀 Tools & Technologies

* **Power BI** – Dashboarding & Visualization
* **Excel** – Data source
* **Python/Pandas** – Data preprocessing (optional)

---

## 📂 How to Use

1. Open the dataset **`BlinkIT Grocery Data.xlsx`** for reference.
2. Load the **`Blinkit data analysis.pbix`** file in **Power BI Desktop**.
3. Refresh data if needed and explore interactive dashboards.

---

✨ This project provides **data-driven insights** into Blinkit’s grocery sales and helps in **strategic decision-making** for product placement, store optimization, and customer satisfaction.

