# E-Commerce Sales Data Preparation, Transformation & Data Modeling using Power Query

## 📌 Project Overview

This project was completed as part of the **Data Analytics (DA) – Module 2** course. The objective was to prepare, clean, transform, and model an E-Commerce sales dataset using **Power Query** and **Power BI**.

The project focuses on data preparation techniques such as importing datasets, transforming data, creating calculated columns, merging tables, handling missing values and duplicates, sorting, filtering, performing aggregations, and establishing relationships between tables for accurate business analysis and reporting.

---

## 📂 Dataset

The project uses the following datasets:

- **List of Orders.csv**
- **Order Details.csv**
- **Sales Target.csv**

---

## 🛠 Tools Used

- Microsoft Power BI
- Power Query
- CSV Datasets

---

## ✅ Tasks Completed

### 1. Data Import

- Imported all three datasets into Power Query Editor.
- Verified successful loading of each dataset.

### 2. Data Transformation

- Limited the **List of Orders** table to the first **500 rows**.
- Converted:
  - **Order Date** → Date
  - **Amount** → Fixed Decimal Number
  - **Target** → Fixed Decimal Number

### 3. Text Formatting

- Converted **Customer Name** values to Proper Case for consistent formatting.

### 4. Custom Columns

Created the following columns:

- **Location** = City + State
- **Profit Margin** = Profit ÷ Amount (formatted as Percentage)

### 5. Conditional Column

Created a **Profit Status** column using the following logic:

- Profit < 0 → **Loss**
- Profit = 0 → **Break-Even**
- Profit > 0 → **Profit**

### 6. Data Merging

Merged:

- **List of Orders**
- **Order Details**

using **Order ID** to create the **Orders Data** table.

### 7. Data Cleaning

Performed data quality checks by:

- Identifying missing values
- Replacing or removing missing values where appropriate
- Removing duplicate records
- Retaining valid transactional duplicates when required

### 8. Sorting & Filtering

- Sorted data by **Order Date** in descending order.
- Filtered records for **Tamil Nadu** to perform state-specific analysis.

### 9. Grouping & Aggregation

Performed the following aggregations:

- Count of Order IDs
- Average Profit by Category
- Total Amount by Sub-Category
- Total Sales Target by Month

### 10. Data Modeling

Established relationships between the datasets using **Power BI Model View**.

#### Relationship 1

- **List of Orders** → **Order Details**
- Common Key: **Order ID**
- Cardinality: **One-to-Many (1:*)**
- Cross Filter Direction: **Single**

#### Relationship 2

- **Sales Target** → **Order Details**
- Common Key: **Category**
- Cardinality: **One-to-Many (1:*)**
- Cross Filter Direction: **Single**

Verified both relationships using **Manage Relationships** to ensure they were active and correctly configured for accurate analysis and reporting.

---

## 📊 Project Outcome

The project resulted in a clean, structured, and analysis-ready data model by applying data preparation, transformation, and modeling techniques in Power BI. The datasets were successfully cleaned, merged, aggregated, and connected through active relationships, enabling accurate analysis, DAX calculations, and interactive business reporting.

---

## 👤 Author

**Maathangi**
