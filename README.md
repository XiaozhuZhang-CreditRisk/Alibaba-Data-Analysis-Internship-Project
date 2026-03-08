# E-commerce User Behavior Analysis

## Project Overview

This project analyzes large-scale e-commerce user behavior data to understand customer engagement, product performance, and purchasing patterns. The objective is to identify actionable insights that can improve conversion rates, customer retention, and product strategy.

The analysis covers over **140,000 customers and 52,000 products**, using exploratory data analysis, customer segmentation, funnel modeling, and time-based behavioral analysis.

This project demonstrates practical data analysis skills including **EDA, customer segmentation, funnel analysis, and data visualization**.

---

## Project Highlights

- Analyzed **140,715 customers** and **52,950 products**
- Built a **user behavior funnel (PageView → SavedCart → Order)**
- Performed **customer segmentation using RF scoring**
- Identified **daily peak activity hours**
- Generated **data-driven business recommendations for conversion optimization**

---

## Dataset

The dataset contains anonymized e-commerce user behavior logs, including:

- Page view events
- Add-to-cart actions
- Purchase orders
- Product identifiers
- User activity timestamps

**Dataset Scale:**
- **140,715 unique customers**
- **52,950 products**
- Multiple interaction events across browsing and purchasing stages

This dataset reflects typical online shopping behavior and allows analysis of customer journeys and purchasing patterns.

---

## Project Structure

The analysis is organized into five sequential Jupyter notebooks:

- `01-basic-stats.ipynb`: Basic statistical analysis and data exploration
- `02-activity-funnel-model.ipynb`: User activity funnel analysis
- `03-top20-products-rf-score.ipynb`: Top products analysis with RF scoring
- `04-hourly-activity-chart.ipynb`: Hourly activity patterns visualization
- `05-data-analysis.ipynb`: Comprehensive data analysis and insights

Each notebook builds upon insights from the previous stage.

---

## Analysis Modules

### 1. Basic Statistics

Initial exploration of the dataset focusing on data quality, customer/product counts, and baseline conversion metrics.

**Key Metrics:**
- Total customers: **140,715**
- Total products: **52,950**
- Average page views per customer: **1.17**
- Average orders per customer: **0.08**

**Conversion Rates:**
- PageView → Order: **8.56%**
- PageView → SavedCart: **2.35%**

---

### 2. Activity Funnel Analysis

A behavioral funnel was constructed to analyze the user journey from browsing to purchase (`PageView → SavedCart → Order`).

**Key Insights:**
- Identification of major **drop-off points** between stages.
- Evaluation of **conversion performance** to pinpoint friction areas.
- Strategic opportunities to improve **checkout completion**.

<p align="center">
  <img src="https://github.com/user-attachments/assets/227a5eda-105f-4e8a-8363-50d8e186a881" width="600" alt="User Behavior Funnel Chart">
  <br>
  <em>Figure 1: User Behavior Funnel (PageView → SavedCart → Order)</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/f35df29c-e645-4d91-95a5-4f1a12a43463" width="600" alt="Funnel Conversion Rates">
  <br>
  <em>Figure 2: Detailed Conversion Rates at Each Stage</em>
</p>

---

### 3. Product Performance Analysis

Top-performing products were identified based on user engagement and purchasing behavior to guide inventory and marketing strategies.

**Analysis Includes:**
- Top products by total views
- Top products by total orders
- Engagement vs. conversion comparison

**Strategic Value:**
- Identifies **high-interest products** needing stock assurance.
- Highlights **high-conversion products** for featured placement.
- Flags **underperforming products** requiring listing optimization.

---

### 4. Customer Segmentation (RF Scoring)

Customers were segmented using an **RF (Recency, Frequency) scoring model** to tailor marketing efforts.

- **Recency (R)**: How recently a customer purchased.
- **Frequency (F)**: How often a customer purchases.

**Customer Segments:**
- **High Value** (RF ≥ 8): 2,479 customers
- **Medium Value** (RF 5–7): 33,853 customers
- **Low Value** (RF < 5): 104,383 customers

**Distribution:**
- **2%** High Value
- **24%** Medium Value
- **74%** Low Value

<p align="center">
  <img src="https://github.com/user-attachments/assets/58e123e0-15bc-4de5-b91b-a41640884a63" width="700" alt="RF Score Distribution">
  <br>
  <em>Figure 3: Customer Distribution by RF Score Segment</em>
</p>

---

### 5. Time-based Activity Analysis

User activity patterns were analyzed across different hours and days to optimize marketing timing and support staffing.

**Key Insights:**
- Identification of **peak activity hours** for traffic surges.
- Distinct differences between **browsing** and **purchasing** behaviors over time.
- Clear **daily and weekly engagement patterns**.

<p align="center">
  <img src="https://github.com/user-attachments/assets/2be3c361-bce2-4fae-9522-d6e56c1ae1c2" width="700" alt="Hourly Activity Overview">
  <br>
  <em>Figure 4: Hourly User Activity Trends</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/511b8561-2692-4a28-8ed0-f7de6beac9f0" width="700" alt="Browsing vs Buying Heatmap">
  <br>
  <em>Figure 5: Heatmap of Browsing vs. Buying Behavior</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/023137a5-64d8-4d14-846e-42f9a8efccb4" width="700" alt="Weekday vs Weekend Patterns">
  <br>
  <em>Figure 6: Weekday vs. Weekend Activity Comparison</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/b772c368-fa94-4af2-8b82-ffbca411f215" width="700" alt="Peak Hour Conversion">
  <br>
  <em>Figure 7: Conversion Rates During Peak Hours</em>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/f062ac02-d34b-44e3-b059-1b6b80b7e5b6" width="700" alt="Time Series Analysis">
  <br>
  <em>Figure 8: Detailed Time-Series Activity Breakdown</em>
</p>

---

## Key Insights

### Customer Behavior
- Strong browsing behavior but relatively **low purchase frequency**.
- Most customers are **infrequent buyers**, indicating a need for retention strategies.
- Significant opportunity exists to improve **browsing-to-purchase conversion**.

### Product Performance
- Top products contribute a **large share of total orders** (Pareto Principle).
- Some high-traffic products show **low conversion rates**, suggesting listing optimization opportunities.

### Customer Segmentation
- A small percentage (**2%**) of customers generate **high purchasing value**.
- Medium-value customers represent strong **growth potential** for upselling.

### User Activity Patterns
- Clear **daily peaks in browsing activity** identified.
- Purchase behavior follows **distinct time patterns**, allowing for timed promotions.

---

## Business Recommendations

### 1. Conversion Optimization
- Reduce friction between **PageView and SavedCart** (e.g., simplify UI, add trust badges).
- Implement **retargeting strategies** (emails/push notifications) for users who abandon carts.

### 2. Customer Retention
- Develop **loyalty programs** specifically for High and Medium Value customers.
- Launch **re-engagement campaigns** (discounts, new arrival alerts) for Low Value users.

### 3. Product Strategy
- Promote **high-converting products** on the homepage.
- Analyze and improve listings (images, descriptions, reviews) for **high-view but low-conversion products**.

### 4. Marketing Timing
- Schedule marketing campaigns and push notifications during **peak activity hours**.
- Optimize customer support availability based on identified **traffic surges**.

---

## Tech Stack

- **Languages**: Python
- **Data Manipulation**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Machine Learning**: Scikit-learn (for RF Scoring)
- **Environment**: Jupyter Notebook

**Core Techniques:**
- Exploratory Data Analysis (EDA)
- Behavioral Funnel Analysis
- Customer Segmentation (RF Model)
- Time-Series Analysis

---

## Author

**Xiaozhu Zhang**  
M.S. Enterprise Risk Management, Columbia University  
*Focus: Risk Management, Credit Risk Analysis & Risk Consulting*
