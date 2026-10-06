# Bank Marketing — Exploratory Data Analysis & Interactive Dashboard

## 📊 Project Overview

This project focuses on analyzing the **Bank Marketing dataset** to understand customer characteristics, marketing campaign performance, and factors associated with term deposit subscriptions.

The project uses **Excel, Power Query, Power BI, and DAX** to perform data cleaning, transformation, exploratory data analysis, visualization, and interactive dashboard development.

The final result is a **4-page interactive Power BI dashboard** that provides insights into customer demographics, campaign performance, contact methods, and subscription behavior.

---

## 🎯 Objectives

- Clean and prepare the Bank Marketing dataset.
- Explore customer demographic and financial characteristics.
- Analyze marketing campaign performance.
- Understand customer subscription behavior.
- Identify patterns across customer groups and contact methods.
- Create interactive dashboards using Power BI.
- Generate meaningful business insights from the data.

---

## 📁 Dataset

**Dataset:** Bank Marketing Dataset

**Source:** UCI Machine Learning Repository

The dataset contains information about customers contacted during a bank marketing campaign.

### Dataset Features

| Feature | Description |
|---|---|
| age | Age of the customer |
| job | Type of occupation |
| marital | Marital status |
| education | Education level |
| default | Whether the customer has credit in default |
| balance | Average yearly balance |
| housing | Whether the customer has a housing loan |
| loan | Whether the customer has a personal loan |
| contact | Contact communication type |
| day | Day of the month of last contact |
| month | Month of last contact |
| duration | Duration of the last contact |
| campaign | Number of contacts during the current campaign |
| pdays | Number of days since previous contact |
| previous | Number of contacts before the current campaign |
| poutcome | Outcome of the previous marketing campaign |
| y | Whether the customer subscribed to a term deposit |

---

## 🛠️ Tools & Technologies

- **Microsoft Excel**
- **Power Query**
- **Microsoft Power BI**
- **DAX**

---

## 🧹 Data Cleaning & Transformation

The dataset was cleaned and prepared using **Power Query**.

### Cleaning steps included:

- Checked for missing and null values.
- Replaced `unknown` values with `Not Specified`.
- Checked for errors.
- Removed duplicate records.
- Validated numerical ranges.
- Validated categorical values.
- Renamed the `y` column to **Subscription Status**.
- Created age groups using Power BI bins.
- Verified appropriate data types for numerical and categorical columns.

---

## 📈 Power BI Dashboard

The dashboard consists of four interactive pages.

### 1. Executive Overview

Provides a high-level summary of the dataset and marketing campaign.

**Key KPIs:**
- Total Customers
- Average Age
- Average Balance
- Subscribed Customers
- Subscription Rate

**Visualizations:**
- Customer Subscription Status
- Subscribed Customers by Job
- Subscription Rate by Job
- Customer Distribution by Education
- Customer Distribution by Marital Status
- Subscription Status by Contact Method
- Subscription Rate by Contact Method

---

### 2. Customer Analysis

Focuses on customer demographics, employment, loans, and financial characteristics.

**Visualizations:**
- Customer Distribution by Age Group
- Customer Distribution by Job
- Customer Distribution by Education
- Customer Distribution by Marital Status
- Average Balance by Job
- Housing Loan Status
- Personal Loan Status

---

### 3. Campaign Analysis

Analyzes marketing campaign activity and previous campaign outcomes.

**Visualizations:**
- Customers by Contact Method
- Average Call Duration by Contact Method
- Customer Distribution by Campaign Contacts
- Previous Campaign Outcome
- Subscription Rate by Previous Campaign Outcome
- Campaign Contacts vs Subscription Rate

---

### 4. Relationship Analysis

Examines relationships between customer characteristics, campaign metrics, and subscription behavior.

**Visualizations:**
- Average Balance by Age Group
- Average Call Duration by Age Group
- Average Balance by Subscription Status
- Average Call Duration by Subscription Status
- Subscription Rate by Age Group

---

## 📌 Key Insights

Some important findings from the analysis include:

- The majority of customers were contacted through **cellular communication**.
- A relatively small proportion of customers subscribed to the term deposit.
- Customers with a **successful previous campaign outcome** showed a substantially higher subscription rate.
- **Subscribed customers had considerably longer average call durations** than non-subscribed customers.
- Customer balance varies across different age groups and subscription statuses.
- Customers with different employment and education backgrounds show different subscription patterns.
- Campaign contact frequency shows differences in subscription rates across customer groups.

> These observations indicate associations in the dataset and should not be interpreted as direct causal relationships.

---

## 📊 Interactive Features

The dashboard includes interactive slicers for:

- **Job**
- **Education**
- **Marital Status**

The slicers are synchronized across all four dashboard pages, allowing users to explore the analysis from different customer perspectives.

---

## 🧮 DAX Measures

Several DAX measures were created for the analysis, including:

```DAX
Total Customers =
COUNTROWS('Bank Marketing')
