# Customer Sentiment & Service Experience Analysis

## 📘 Project Overview
This project presents an **end-to-end customer sentiment and service experience analysis** using Python.  
It aims to understand how **customer emotions, ratings, response time, complaint behavior, and issue resolution** collectively shape customer satisfaction and operational service risk.

The analysis integrates structured data processing, feature engineering, statistical summarization, and advanced visual analytics to deliver **actionable, business-driven insights** for improving customer support performance.

---

## 🎯 Project Objectives
The primary objectives of this project are to:

1. Analyze the overall distribution of customer sentiment (Positive, Neutral, Negative)
2. Examine alignment and misalignment between customer ratings and expressed sentiment
3. Evaluate the impact of response time on customer satisfaction
4. Identify response-time thresholds that escalate negative sentiment
5. Study how complaint registration varies across sentiment categories
6. Assess the effect of issue resolution on customer perception
7. Identify **silent dissatisfied customers** who do not register complaints
8. Compare sentiment across platforms, product categories, regions, age groups, and gender
9. Develop a **custom service risk score** to quantify operational risk
10. Build a visual dashboard integrating sentiment and service metrics
11. Derive data-driven recommendations for customer support optimization

---

## 🗂️ Dataset Description
The dataset represents **customer feedback and service interaction records** collected across multiple platforms and product categories.

- Each row corresponds to **one customer interaction or review**
- The dataset combines **demographic, behavioral, service, and feedback attributes**
- Both qualitative (sentiment, review text) and quantitative (ratings, response time) variables are included

---

## 📊 Table Structure (Data Dictionary)

| Column Name | Data Type | Description | Analytical Relevance |
|------------|----------|-------------|----------------------|
| `customer_id` | Integer / String | Unique identifier for each customer | Record tracking and deduplication |
| `age_group` | Categorical | Age range of the customer | Demographic sentiment comparison |
| `gender` | Categorical | Gender of the customer | Gender-based perception analysis |
| `region` | Categorical | Geographic region of the customer | Regional service performance |
| `platform` | Categorical | Platform used (Web, App, Store, etc.) | Platform-wise sentiment & response |
| `product_category` | Categorical | Category of purchased product | Product-level service evaluation |
| `purchase_channel` | Categorical | Mode of purchase | Channel-based service assessment |
| `review_text` | Text | Written customer feedback | Basis for sentiment classification |
| `sentiment` | Categorical | Sentiment label (positive / neutral / negative) | Core emotional indicator |
| `customer_rating` | Numeric (1–5) | Customer satisfaction rating | Quantitative satisfaction measure |
| `response_time_hours` | Numeric | Support response time in hours | Key service performance metric |
| `complaint_registered` | Binary (Yes/No) | Complaint filing indicator | Complaint behavior analysis |
| `issue_resolved` | Binary (Yes/No) | Issue resolution status | Resolution impact measurement |

---

## 🧹 Data Cleaning & Standardization
To ensure analytical reliability:

- Missing categorical values were replaced with `"unknown"`
- Text fields were standardized (lowercase, trimmed)
- Binary columns normalized to consistent `yes / no` values
- Duplicate records removed to prevent bias

This step ensures **consistency, accuracy, and reproducibility**.

---

## 🧠 Feature Engineering

### 🔹 Review Length
- Calculated as the character length of `review_text`
- Used to assess emotional intensity in customer feedback

### 🔹 Response Time Buckets
Response time was categorized into operational thresholds:

| Bucket | Interpretation |
|------|---------------|
| `<1h` | Immediate response |
| `1–3h` | Fast response |
| `3–6h` | Acceptable delay |
| `6–12h` | High delay |
| `12–24h` | Critical delay |
| `>24h` | Severe service failure |

These buckets enable **threshold-based sentiment analysis**.

---

## ❓ Business & Analytical Questions
- What is the emotional distribution of customers?
- Do customer ratings always reflect sentiment?
- How does delayed support affect customer perception?
- Which response-time thresholds increase dissatisfaction?
- Are unresolved issues strong drivers of negative sentiment?
- How many dissatisfied customers remain silent?
- Which platforms and product categories show higher service risk?
- How does sentiment vary across demographics and regions?
- Can service risk be quantified numerically?

---

## 📈 Analytical Components

### 🔹 Sentiment Distribution
- Absolute and percentage breakdown of sentiment categories
- Indicates overall customer emotional health

### 🔹 Rating–Sentiment Alignment
- Average rating by sentiment
- Identification of misaligned cases:
  - High rating with negative sentiment
  - Low rating with positive sentiment

### 🔹 Response Time Impact
- Average response time by sentiment
- Cross-analysis using response-time buckets

### 🔹 Complaint Analysis
- Complaint registration across sentiment categories
- Identifies underreported dissatisfaction

### 🔹 Issue Resolution Impact
- Sentiment comparison for resolved vs unresolved cases
- Highlights the importance of closure in service delivery

### 🔹 Demographic & Regional Analysis
- Sentiment variation by age group and gender
- Regional response time and rating comparison

---

## 🚨 Silent Dissatisfaction
Customers with:
- `sentiment = negative`
- `complaint_registered = no`

were classified as **silent dissatisfied customers**.

These customers represent **hidden churn risk** and are not visible in complaint-based monitoring systems.

---

## ⚠️ Service Risk Score
A composite **Service Risk Score** was developed:


### Purpose:
- Quantify operational service risk
- Identify high-risk interactions
- Enable proactive customer support intervention

---

## 📊 Visualization & Dashboard
A consolidated dashboard was created to visualize:
- Sentiment distribution
- Average ratings by sentiment
- Response time patterns
- Complaint behavior
- Issue resolution share
- Platform-wise service performance

Designed for **managerial and executive decision-making**.

---

## 🔍 Key Insights
1. Positive sentiment aligns with faster responses and higher ratings
2. Delayed response and unresolved issues strongly drive negative sentiment
3. Rating–sentiment misalignment reveals hidden dissatisfaction
4. A significant proportion of dissatisfied customers remain silent
5. Certain platforms and product categories consistently show higher risk
6. Issue resolution has a major positive impact on sentiment
7. Service risk score effectively highlights operational bottlenecks

---

## ✅ Recommendations
- Reduce response time beyond the **3–6 hour threshold**
- Prioritize quick issue resolution
- Monitor silent dissatisfaction using sentiment data
- Use service risk scores to flag high-risk cases
- Improve service quality on high-risk platforms and products
- Regularly monitor dashboards for early warning signals

---

## 🛠️ Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

---

## 📁 Suggested Project Structure

---

## 👤 Author
**Supratim Maity**    

---

⭐ If you find this project useful, consider starring the repository.
