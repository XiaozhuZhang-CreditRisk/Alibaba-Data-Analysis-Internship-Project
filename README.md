# E-commerce User Behavior Analysis

## Project Overview

This project analyzes large-scale e-commerce user behavior data to understand customer engagement, product performance, and purchasing patterns. The objective is to identify actionable insights that can improve conversion rates, customer retention, and product strategy.

The analysis covers over **140,000 customers and 52,000 products**, using exploratory data analysis, customer segmentation, funnel modeling, and time-based behavioral analysis.

This project demonstrates practical data analysis skills including **EDA, customer segmentation, funnel analysis, and data visualization**.

---

## Project Highlights

• Analyzed **140,715 customers** and **52,950 products**
• Built a **user behavior funnel (PageView → SavedCart → Order)**
• Performed **customer segmentation using RF scoring**
• Identified **daily peak activity hours**
• Generated **data-driven business recommendations for conversion optimization**

---

## Dataset

The dataset contains anonymized e-commerce user behavior logs, including:

* Page view events
* Add-to-cart actions
* Purchase orders
* Product identifiers
* User activity timestamps

Dataset scale:

* **140,715 unique customers**
* **52,950 products**
* Multiple interaction events across browsing and purchasing stages

This dataset reflects typical online shopping behavior and allows analysis of customer journeys and purchasing patterns.

---

## Project Structure

The analysis is organized into five sequential Jupyter notebooks:

```
01-basic-stats.ipynb
02-activity-funnel-model.ipynb
03-top20-products-rf-score.ipynb
04-hourly-activity-chart.ipynb
05-data-analysis.ipynb
```

Each notebook builds upon insights from the previous stage.

---

## Analysis Modules

### 1. Basic Statistics

Initial exploration of the dataset.

Key analysis:

* Data overview and quality assessment
* Customer and product statistics
* Conversion rate calculations
* Average engagement metrics

Key metrics:

* Total customers: **140,715**
* Total products: **52,950**
* Average page views per customer: **1.17**
* Average orders per customer: **0.08**

Conversion rates:

* PageView → Order: **8.56%**
* PageView → SavedCart: **2.35%**

---

### 2. Activity Funnel Analysis

A behavioral funnel was constructed to analyze the user journey from browsing to purchase.

Funnel stages:

PageView → SavedCart → Order

Key insights:

* Identification of major **drop-off points**
* Evaluation of **conversion performance between stages**
* Opportunities to improve **checkout completion**

Layout:
<img width="786" height="492" alt="image" src="https://github.com/user-attachments/assets/227a5eda-105f-4e8a-8363-50d8e186a881" />
<img width="800" height="500" alt="image" src="https://github.com/user-attachments/assets/f35df29c-e645-4d91-95a5-4f1a12a43463" />

---

### 3. Product Performance Analysis

Top-performing products were identified based on user engagement and purchasing behavior.

Analysis includes:

* Top products by views
* Top products by orders
* Engagement vs conversion comparison

This helps identify:

* High-interest products
* High-conversion products
* Underperforming products that require optimization

---

### 4. Customer Segmentation (RF Scoring)

Customers were segmented using an **RF scoring model**.

Recency (R): how recently a customer purchased
Frequency (F): how often a customer purchases

Customer segments:

High Value Customers (RF ≥ 8): **2,479 customers**
Medium Value Customers (RF 5–7): **33,853 customers**
Low Value Customers (RF < 5): **104,383 customers**

Customer distribution:

* **74% Low Value customers**
* **24% Medium Value customers**
* **2% High Value customers**

This segmentation supports targeted marketing strategies.

Layout:
<img width="1576" height="870" alt="image" src="https://github.com/user-attachments/assets/58e123e0-15bc-4de5-b91b-a41640884a63" />

---

### 5. Time-based Activity Analysis

User activity patterns were analyzed across different hours of the day.

Key insights:

* Identification of **peak activity hours**
* Differences between browsing and purchasing behavior
* Daily engagement patterns

Visualizations include:

* Hourly activity charts
* Behavioral heatmaps

Layout:
<img width="1588" height="814" alt="image" src="https://github.com/user-attachments/assets/2be3c361-bce2-4fae-9522-d6e56c1ae1c2" />
<img width="1562" height="622" alt="image" src="https://github.com/user-attachments/assets/511b8561-2692-4a28-8ed0-f7de6beac9f0" />
<img width="1550" height="902" alt="image" src="https://github.com/user-attachments/assets/023137a5-64d8-4d14-846e-42f9a8efccb4" />
<img width="1542" height="742" alt="image" src="https://github.com/user-attachments/assets/b772c368-fa94-4af2-8b82-ffbca411f215" />
<img width="1530" height="890" alt="image" src="https://github.com/user-attachments/assets/f062ac02-d34b-44e3-b059-1b6b80b7e5b6" />

---

## Key Insights

### Customer Behavior

* Strong browsing behavior but relatively **low purchase frequency**
* Most customers are **infrequent buyers**
* Significant opportunity exists to improve **browsing-to-purchase conversion**

### Product Performance

* Top products contribute a **large share of total orders**
* Some high-traffic products show **low conversion rates**, suggesting listing optimization opportunities

### Customer Segmentation

* A small percentage of customers generate **high purchasing value**
* Medium-value customers represent strong **growth potential**

### User Activity Patterns

* Clear **daily peaks in browsing activity**
* Purchase behavior follows **distinct time patterns**

---

## Business Recommendations

### Conversion Optimization

* Reduce friction between **PageView and SavedCart**
* Implement **retargeting strategies** for users who abandon carts

### Customer Retention

* Develop **loyalty programs for high-value customers**
* Launch **re-engagement campaigns** for low-value users

### Product Strategy

* Promote **high-converting products**
* Improve listings for **high-view but low-conversion products**

### Marketing Timing

* Schedule marketing campaigns during **peak activity hours**
* Optimize promotions based on user engagement patterns

---

## Tech Stack

Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Jupyter Notebook

Techniques used:

* Exploratory Data Analysis (EDA)
* Behavioral Funnel Analysis
* Customer Segmentation
* Data Visualization

---

## Author


---
