# E-Commerce Sales Data Preparation and Transformation using Power Query

## 📌 Project Overview

This project was completed as part of the **Data Analytics (DA) – Module 2** course. The objective was to prepare, clean, transform, and analyze an E-Commerce sales dataset using **Power Query**.

The project focuses on data preparation techniques such as importing datasets, transforming data, creating calculated columns, merging tables, handling missing values and duplicates, sorting, filtering, and performing aggregations to generate meaningful business insights.

---

## 📂 Dataset

The project uses the following datasets:

* **List of Orders.csv**
* **Order Details.csv**
* **Sales Target.csv**

---

## 🛠 Tools Used

* Microsoft Power Query (Power BI Service / Microsoft Fabric)
* CSV Datasets

---

## ✅ Tasks Completed

### 1. Data Import

* Imported all three datasets into Power Query Editor.
* Verified successful loading of each dataset.

### 2. Data Transformation

* Limited the List of Orders table to the first **500 rows**.
* Converted:

  * **Order Date** → Date
  * **Amount** → Fixed Decimal Number
  * **Target** → Fixed Decimal Number

### 3. Text Formatting

* Converted **Customer Name** values to Proper Case for consistent formatting.

### 4. Custom Columns

Created the following columns:

* **Location** = City + State
* **Profit Margin** = Profit ÷ Amount (formatted as Percentage)

### 5. Conditional Column

Created a **Profit Status** column using the following logic:

* Profit < 0 → **Loss**
* Profit = 0 → **Break-Even**
* Profit > 0 → **Profit**

### 6. Data Merging

Merged:

* **List of Orders**
* **Order Details**

using **Order ID** to create the **Orders Data** table.

### 7. Data Cleaning

Performed data quality checks by:

* Identifying missing values
* Replacing or removing missing values where appropriate
* Removing duplicate records
* Retaining valid transactional duplicates when required

### 8. Sorting & Filtering

* Sorted data by **Order Date** in descending order.
* Filtered records for **Tamil Nadu** to perform state-specific analysis.

### 9. Grouping & Aggregation

Performed the following aggregations:

* Count of Order IDs
* Average Profit by Category
* Total Amount by Sub-Category
* Total Sales Target by Month

---

## 📊 Project Outcome

The project resulted in a clean, structured, and analysis-ready dataset by applying various data preparation techniques in Power Query. The transformed data can be used for reporting and business analysis.

---

## 📁 Repository Structure

```
📦 power-query-ecommerce-data-transformation
├── README.md
├── Project_Report.pdf
├── Dataset
│   ├── List_of_Orders.csv
│   ├── Order_Details.csv
│   └── Sales_Target.csv
└── Screenshots
    ├── Data_Import.png
    ├── Data_Transformation.png
    ├── Custom_Columns.png
    ├── Data_Merging.png
    ├── Data_Cleaning.png
    ├── Sorting_Filtering.png
    └── Aggregation.png
```

---

## 📌 Note

This project was completed using **Power Query editor**. The **Data Modeling** task (creating relationships and Model View) was not included because Power Query Online does not support Model View or saving projects as **.pbix** files. All required data import, transformation, cleansing, merging, filtering, and aggregation tasks were successfully completed within the available environment.

---

## 👤 Author

Maathangi
