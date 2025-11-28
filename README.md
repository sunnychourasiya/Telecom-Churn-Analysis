# Telecom Customer Churn Analysis
*A Strategic Assessment of Customer Churn & Retention Drivers*

<p align="left">
  <img src="https://img.shields.io/badge/Python-3.9-blue" />
  <img src="https://img.shields.io/badge/Pandas-Data--Processing-yellow" />
  <img src="https://img.shields.io/badge/Seaborn-Visualization-blue" />
  <img src="https://img.shields.io/badge/NumPy-Numerical-green" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-orange" />
</p>

---

## 📌 Project Summary

| Category | Details |
|----------|---------|
| **Domain** | Telecom Customer Analytics |
| **Business Objective** | Identify churn drivers & design actionable retention strategies |
| **Dataset Size** | 7,043 customers × 38 features |
| **Deliverables** | KPIs, segmentation, churn insights, strategic recommendations |
| **Tech Stack** | Python, Pandas, NumPy, Seaborn, Matplotlib |
| **Business Impact** | Reduce churn, increase CLV, improve onboarding, pricing & service |

---

## 📊 Key Highlights at a Glance

- Analyzed **7,000+ customer profiles**  
- Identified **27% churn rate** with early-tenure dominance  
- Discovered **competitor switching** as the leading churn reason (~44%)  
- Found **fiber users** churn significantly more due to competition  
- Uncovered **2–3× higher churn** among customers without add-on services  
- Mapped **55% churn within first-year**, highlighting onboarding gaps  
- Generated **targeted strategies** for Marketing, CX, Product & Strategy teams  

---

## Repository Structure 

```
Telecom-Churn-Analysis/
│
├── data/
│   └── Telecom_Customer_Churn.csv
│
├── notebook/
│   └── CHURN_ANALYSIS.ipynb
│
├── images/
│   ├── Financial_metrics.png
│   ├── status_distribution_pie.png
│   ├── churn_by_city.png
│   ├── churn_by_tenure_category.png
│   ├── churn_reasons.png
│   └── churn_category_distribution.png
│
└── README.md

```

---

## 📘 Table of Contents

| Section | Link |
|--------|------|
| Executive Overview | [Go to Section](#executive-overview) |
| Problem Statement | [Go to Section](#problem-statement) |
| Project Objectives | [Go to Section](#project-objectives) |
| Project Workflow | [Go to Section](#project-workflow) |
| Dataset Description | [Go to Section](#dataset-description) |
| Data Preparation & Cleaning | [Go to Section](#data-preparation--cleaning) |
| Feature Engineering | [Go to Section](#feature-engineering) |
| Exploratory Data Analysis (EDA) | [Go to Section](#exploratory-data-analysis-eda) |
| Key KPI Highlights | [Go to Section](#key-kpi-highlights) |
| Key Insights | [Go to Section](#key-insights) |
| Strategic Recommendations | [Go to Section](#strategic-recommendations) |
| Business Impact | [Go to Section](#business-impact) |
| Results Summary | [Go to Section](#results-summary) |
| Technologies Used | [Go to Section](#technologies-used) |
| Skills Demonstrated | [Go to Section](#skills-demonstrated) |
| Conclusion | [Go to Section](#conclusion) |

---

## Executive Overview

Telecom operators operate in a highly competitive, price-sensitive environment where customer churn directly impacts profitability, market share, and lifetime value. This project provides a structured, data-driven churn analysis to uncover:

- *Which customer segments are most at risk*  
- *What behaviors and service attributes drive churn*  
- *Where customer experience or product gaps exist*  
- *Which strategic levers can effectively reduce attrition*

The analysis translates raw customer data into clear, actionable recommendations aligned with marketing, customer experience (CX), product, and strategy functions.

---

## Problem Statement

Despite high acquisition costs, telecom operators lose a significant share of customers due to:

- Competitive switching (pricing, fiber speed, device upgrades)
- Weak early-life onboarding and value communication
- Service quality and customer experience issues
- Billing complexity and unexpected charges
- Low attachment to add-on services (low stickiness)

Lack of segmentation and visibility into churn drivers limits the effectiveness of retention programs.

---


## Project Objectives

- Identify primary demographic, behavioral & service churn drivers  
- Compare churn vs retention across contract type, charges, add-ons, internet type, tenure  
- Engineer analytical features to enhance churn interpretation  
- Generate actionable insights to assist retention teams  
- Build a foundation for predictive churn modeling  

---

## Project Workflow

```

Raw Data  
   ↓  
Data Cleaning  
   ↓  
Feature Engineering  
   ↓  
Exploratory Data Analysis  
   ↓  
Insights & Churn Drivers  
   ↓  
Strategic Recommendations

```

## Dataset Description

**Source:** Maven Telecom Customer Churn Challenge  
**File:** `Telecom_Customer_Churn.csv`  
**Size:** 7,043 rows × 38 columns  

The dataset captures customer demographics, service subscriptions, billing behavior, and churn outcomes—providing a comprehensive foundation for churn pattern analysis. The features span four key categories:

- **Demographics** → Age, gender, dependents, geography  
- **Account Information** → Tenure, contract type, billing method, payment mode  
- **Service Usage** → Internet type, phone services, add-ons, data consumption  
- **Customer Status** → Active / Churned / Inactive, churn category, churn reason  

### Columns Overview

| **Column**            | **Description**                 | **Data Type** |
|-----------------------|---------------------------------|----------------|
| Customer ID           | Unique customer identifier      | object         |
| Gender                | Male / Female                   | object         |
| Age                   | Customer age                    | int64          |
| Married               | Marital status                  | object         |
| Number of Dependents  | Count of dependents             | int64          |

*This table shows the first five columns.  
A full, detailed data dictionary is available in the notebook (`CHURN_ANALYSIS.ipynb`).*


---


## Data Preparation & Cleaning

**Notebook:** `CHURN_ANALYSIS.ipynb`

### Core Cleaning Activities

- Inspected dataset structure, datatypes, and distribution profiles  
- Managed missing values and inconsistencies  
- Standardized categorical values and corrected mislabeled entries  
- Converted numerical fields stored as strings to appropriate data types  
- Addressed duplicate records and removed redundant fields  
- Validated relationships between tenure, billing fields, and charges  

The cleaned dataset forms the foundation for reliable exploratory analysis.

---

## Feature Engineering

To improve analytical depth and interpretability:

- Tenure Groups(0–12, 12–24, 24–48, etc.) were created to segment customer lifecycle stages
- Categorical attributes were standardized and consolidated for comparison
- Engineered fields were added to capture service bundle usage and customer behavior patterns
- Service-level indicators were transformed to enable clearer churn segmentation

These enhancements significantly improved the detection of churn patterns across customer segments.

---

## Exploratory Data Analysis (EDA)

The EDA focused on understanding customer behavior, churn patterns, and key lifecycle risk indicators.

### Univariate Analysis
- Tenure and monthly charge distributions  
- Contract types and service configurations  
- Core demographic attributes  

### Bivariate Analysis
- Churn relationships across contract type, internet service, and payment method  
- Churn variation by tenure groups and billing levels  

### Multivariate Analysis
- Correlation patterns across financial and service variables  
- Churn behavior across bundled services and customer segments  

### Visualization Summary
- Countplots, histograms, boxplots, bar charts, and correlation heatmaps  
- **Tools Used:** Matplotlib, Seaborn

---

### 📊 Key Visualizations

<table>
  <tr>
    <td align="center">
      <img src="images/customer_status_distribution.png" width="350"><br>
      <sub><b>Customer Status Distribution</b></sub>
    </td>
    <td align="center">
      <img src="images/top_cities_churn.png" width="350"><br>
      <sub><b>Top Cities by Churned Customers</b></sub>
    </td>
  </tr>

  <tr>
    <td align="center">
      <img src="images/churn_by_tenure.png" width="350"><br>
      <sub><b>Churn by Tenure Category</b></sub>
    </td>
    <td align="center">
      <img src="images/churn_reasons.png" width="350"><br>
      <sub><b>Churn Reasons</b></sub>
    </td>
  </tr>

  <tr>
    <td align="center">
      <img src="images/churn_category_distribution.png" width="350"><br>
      <sub><b>Churn Category Distribution</b></sub>
    </td>
    <td align="center">
      <img src="images/financial_metrics_by_status.png" width="350"><br>
      <sub><b>Financial Metrics by Customer Status</b></sub>
    </td>
  </tr>
</table>

## Key KPI Highlights

| KPI | Value | Interpretation | Recommended Action |
|------|--------|----------------|--------------------|
| **Overall Churn Rate** | ~27%  | Higher than industry benchmark | Prioritize churn-reduction strategy |
| **First-Month Churn** | Very High | Weak onboarding experience | Strengthen welcome journey |
| **Fiber Optic Churn** | High  | Competitor pressure | Improve pricing & fiber reliability |
| **Churn Within First Year** | 55% | Early lifecycle churn | Enhance early engagement |
| **Add-On Deficit Churn** | 2–3× Higher | Low stickiness | Promote bundled add-ons |
| **Competitor Churn** | ~44% | High competitive threat | Launch loyalty/anti-switch programs |

---

## Key Insights

### **1. Customer Profile & Demographics**
- Churn is highest in **San Diego** and **Los Angeles**  
- **Single / non-married customers** churn more; married customers are more stable  
- **Low long-distance usage** signals early disengagement

### **2. Contract & Tenure Patterns**
- **Month-to-month plans** show the highest churn  
- **55% of churn occurs within the first year**, with a major spike in the **first month**  
- **Family / multi-line plans** reduce churn compared to single-line usage  

### **3. Services, Add-Ons & Competitor Influence**
- **Fiber Optic users** churn at higher rates  
- Lack of **add-ons** (security, backup, device protection, tech support) increases churn  
- **Competitor switching** is the leading churn driver due to better offers, devices, speeds, and data plans  

### **4. Pricing, Billing & Customer Experience**
- Churned customers had **higher monthly charges** but **lower lifetime revenue**  
- **Poor customer service** caused ~310 churn cases  
- **Bank withdrawal** and **paperless billing** users churn more  
- Retained customers often received **refunds or adjustments**, indicating issue resolution supports retention  

---

## Strategic Recommendations

### 1. Strengthen Early Lifecycle Experience
- Proactive onboarding journeys (first 30–60 days)
- First-month bill clarity & proactive communication
- Personalized usage tips & service activation support

### 2. Improve Service Value & Stickiness
- Bundle essential add-ons at discounted rates
- Promote device protection, security & backup services
- Create strong family/multi-line value propositions

### 3. Reduce Competitor Switching
- Loyalty programs targeting high-risk clusters
- Upgrades for fiber customers (speed, pricing, devices)
- Competitor-aware retention offers

### 4. Enhance Customer Service Excellence
- Track top complaint categories and eliminate root causes
- Improve first-contact resolution rates
- Prioritize high-value customers with premium support

### 5. Increase Billing Transparency
- Clear breakdown of monthly charges
- Predictive bill notifications
- Alerts for unusual usage or additional fees

---

## Business Impact

This analysis supports telecom leaders in:

- Reducing churn through high-impact interventions
- Improving onboarding effectiveness
- Strengthening competitive differentiation
- Increasing ARPU and customer lifetime value
- Prioritizing investments in service quality and add-ons
- Identifying at-risk customer clusters for targeted campaigns

---

## Results Summary

- Churn driven primarily by contract type, pricing, service add-ons, and fiber competitiveness
- Clear early-tenure vulnerability across customer base
- Competitor switching accounts for a significant share of churn
- Multi-team, actionable retention roadmap developed
- Dataset fully prepared for predictive modeling & BI dashboards

---

## Technologies Used

- **Python** – Analysis  
- **Pandas** – Data wrangling  
- **NumPy** – Numerical operations  
- **Matplotlib & Seaborn** – Visualization  
- **Jupyter Notebook** – Workflow environment  

---

## Skills Demonstrated

- Data Preparation & Cleaning
- Feature Engineering
- Exploratory Data Analysis
- Visualization & Pattern Recognition
- Telecom Domain Understanding
- Business Strategy Formulation

---

## Conclusion

This analysis provide telecom organizations with a clear understanding of the behavioral, financial, and service factors driving customer attrition. The insights and recommendations provided enable data-driven decision-making across marketing, customer experience, product, and strategy teams—ultimately improving retention, revenue, and customer lifetime value.

---

## ⭐ Support
If you found this project useful, please ⭐ the repository!
