# 🧹 Excel Data Cleaning & Transformation

## 📌 Project Overview

This project focuses on **data cleaning and preparation using Microsoft Excel**.

Real-world datasets often contain missing values, inconsistent text formats, duplicate records, and poorly structured data. Before performing analysis, these issues need to be identified and corrected to improve data quality and reliability.

In this project, I applied Excel data cleaning, transformation, formatting, and conditional formatting techniques to prepare a **Product Dataset** for further analysis.

This project is part of my learning journey as an **Aspiring Data Analyst**.

---

## 🎯 Project Objectives

The main objectives of this project are:

* Identify and handle missing values
* Detect and correct inconsistent data
* Standardize text formats
* Identify and remove duplicate records
* Split and merge columns
* Format dates and numerical values
* Apply conditional formatting
* Improve the overall quality and readability of the dataset

---

## 📂 Dataset

### Dataset: Product Dataset

The dataset contains information about different products.

### Attributes

| Column       | Description                                              |
| ------------ | -------------------------------------------------------- |
| Product ID   | Unique identifier containing product-related information |
| Product Name | Name of the product                                      |
| Brand Name   | Brand associated with the product                        |
| Quantity     | Available quantity                                       |
| Category     | Product category                                         |
| Price        | Price of the product                                     |

---

# 🛠️ Data Cleaning & Transformation Tasks

## 1. Handling Missing Values

### 🔹 Missing Price Values

Checked the **Price** column for missing values.

For products with missing price information, the appropriate strategy is to:

* Identify the missing records
* Avoid assigning arbitrary values
* If possible, use reliable business information or reference data to determine the correct price
* If the value cannot be determined, retain it as missing and document the issue before analysis

### 🔹 Missing Category Values

Checked the **Category** column for missing values.

A suitable approach is to:

* Identify products with missing categories
* Use Product Name or Brand Name to determine the appropriate category where possible
* If the category cannot be reliably determined, classify it as **Unknown** or **Uncategorized**

---

# 2. Correcting Inconsistent Data

## 🔹 Product Name Standardization

Inspected the **Product Name** column for inconsistent text formats such as:

* Different capitalization
* Inconsistent spelling
* Extra spaces
* Variations of the same product name

Used Excel's **Find and Replace** feature to standardize product names.

### Example

```text
Before:
iphone 14
IPHONE 14
IPhone 14

After:
iPhone 14
```

---

## 🔹 Category Correction

Checked the **Category** column for spelling mistakes and inconsistent category names.

Used **Find and Replace** to correct typos and standardize category values.

### Example

```text
Before:
Electonics

After:
Electronics
```

This ensures that the same category is represented consistently throughout the dataset.

---

# 3. Removing Duplicate Records

Checked the complete dataset for duplicate rows based on **all columns**.

Used Excel's:

**Data → Remove Duplicates**

to identify and remove duplicate records where necessary.

This helps prevent duplicate records from affecting future calculations and analysis.

---

# 4. Splitting and Merging Data

## 🔹 Splitting Product ID

The **Product ID** contains multiple pieces of information.

The Product ID was split into:

* Manufacturing Date
* Country Code

Unnecessary characters were removed during the transformation.

### Example

```text
Product ID
28-JAN-US
```

was transformed into separate fields:

| Manufacturing Date | Country Code |
| ------------------ | ------------ |
| 28-JAN             | US           |

The extracted date information was then formatted appropriately.

---

## 🔹 Merging Brand Name and Product Name

Created a new column named **Product Brand** by combining:

* Brand Name
* Product Name

### Excel Formula

```excel
=CONCAT(B2," ",C2)
```

or:

```excel
=B2&" "&C2
```

### Example

```text
Brand Name: Apple
Product Name: iPhone 14

Product Brand:
Apple iPhone 14
```

---

# 5. Number & Date Formatting

## 🔹 Price Formatting

Formatted the **Price** column as currency to improve readability and clearly represent monetary values.

Example:

```text
1000
```

was displayed as:

```text
$1,000.00
```

---

## 🔹 Manufacturing Date Formatting

Formatted the **Manufacturing Date** column to display dates in:

```text
DD-MM-YYYY
```

Example:

```text
28-01-2026
```

This creates a consistent date format across the dataset.

---

# 6. Conditional Formatting

## 🔹 Price Column

Applied **Conditional Formatting** to the Price column using:

* Data Bars
* Color Scales

This provides a visual representation of product prices and makes it easier to identify relatively high and low values.

---

## 🔹 Electronics Category

Created a custom conditional formatting rule for the **Category** column.

The rule highlights cells where:

```text
Category = Electronics
```

This makes Electronics products easy to identify visually.

---

# 📊 Data Cleaning Techniques Used

| Task                  | Excel Technique            |
| --------------------- | -------------------------- |
| Missing Values        | Data inspection & handling |
| Text Standardization  | Find & Replace             |
| Category Correction   | Find & Replace             |
| Duplicate Removal     | Remove Duplicates          |
| Column Splitting      | Text to Columns            |
| Column Merging        | CONCAT / `&`               |
| Price Formatting      | Currency Format            |
| Date Formatting       | Custom Date Format         |
| Price Visualization   | Data Bars / Color Scales   |
| Category Highlighting | Conditional Formatting     |

---

# 🛠️ Excel Skills Demonstrated

Through this project, I practiced:

* Data Cleaning
* Data Preprocessing
* Data Transformation
* Missing Value Handling
* Duplicate Detection
* Text Standardization
* Find and Replace
* Text to Columns
* Column Merging
* Date Formatting
* Currency Formatting
* Conditional Formatting
* Data Quality Improvement

---

# 📁 Project Structure

```text
Excel-Data-Cleaning/
│
├── README.md
│
└── Assignment_2_Data_Cleaning_and_Transformation.xlsx
```

---

# 🎓 Learning Outcome

This project helped me understand that **data cleaning is an important step before performing data analysis**.

I learned how to identify common data quality issues, standardize inconsistent information, remove duplicates, restructure columns, and apply appropriate formatting to make datasets easier to analyze.

This project strengthened my practical Excel skills and forms part of my growing **Data Analyst portfolio**.

---

## 👩‍💻 About Me

I am an **Aspiring Data Analyst** building my skills through hands-on projects and practical datasets.

My current learning journey includes:

**Excel → SQL → Python → Power BI → Data Analytics Projects**

I am continuously building projects to develop my technical and analytical skills and create a strong Data Analyst portfolio.
