# Customer Sentiment & Service Experience Analysis

## 📘 Introduction
In modern customer-centric organizations, understanding **how customers feel** is as important as knowing **what they rate**.  
This project delivers a **comprehensive, end-to-end analytical framework** to study customer sentiment and service experience using Python.

The analysis integrates **sentiment, ratings, response time, complaints, and issue resolution** into a unified view, enabling organizations to:
- Detect dissatisfaction early
- Quantify service risk
- Optimize customer support operations using data-driven insights

---

## 🧩 Problem Context
Customer dissatisfaction often remains hidden behind:
- Neutral or misleading ratings
- Unregistered complaints
- Delayed support responses
- Unresolved service issues

Traditional dashboards focus on surface metrics (ratings, ticket counts), but fail to capture **emotional sentiment** and **silent dissatisfaction**.  
This project bridges that gap.

---

## 🎯 Project Objectives
The core objectives of this project are to:

1. Analyze the **distribution of customer sentiment** (Positive, Neutral, Negative)
2. Evaluate **alignment and misalignment** between ratings and sentiment
3. Measure the **impact of response time** on sentiment
4. Identify **critical response-time thresholds** that increase dissatisfaction
5. Assess how **complaint registration** varies across sentiment types
6. Measure the effect of **issue resolution** on customer perception
7. Detect **silent dissatisfied customers** who did not register complaints
8. Compare sentiment patterns across:
   - Platforms
   - Product categories
   - Regions
   - Age groups
   - Gender
9. Develop a **custom service risk score** for operational risk assessment
10. Build an **integrated visual dashboard** for executive-level insights
11. Derive **actionable business recommendations**

---

## ❓ Key Business Questions Answered
- What proportion of customers are genuinely satisfied or dissatisfied?
- Do high ratings always imply positive sentiment?
- How does delayed support affect customer emotion?
- At what response-time point does sentiment sharply deteriorate?
- Are unresolved issues strongly linked to negative sentiment?
- How many unhappy customers remain silent?
- Which platforms and products pose the highest service risk?
- How do demographics influence service sensitivity?
- Can customer service risk be quantified numerically?

---

## 🧠 Methodology & Analytical Workflow

### 1️⃣ Data Ingestion
- Dataset loaded using **Pandas**
- Shape, schema, and data types examined
- Initial quality checks performed

---

### 2️⃣ Data Cleaning & Standardization
- Missing categorical values replaced with `"unknown"`
- Text fields standardized (lowercase, trimmed)
- Binary columns normalized (`yes/no`)
- Duplicate records removed to ensure data integrity

This step ensures **consistency, accuracy, and analytical reliability**.

---

### 3️⃣ Feature Engineering
New analytical features created:

- **Review Length**  
  Measures depth of customer feedback

- **Response Time Buckets**  
  Categorized response times into:
  - `<1h`
  - `1–3h`
  - `3–6h`
  - `6–12h`
  - `12–24h`
  - `>24h`

These features enable threshold-based behavioral analysis.

---

### 4️⃣ Sentiment Distribution Analysis
- Absolute sentiment counts
- Percentage contribution of each sentiment category
- Identifies overall emotional tone of customers

---

### 5️⃣ Rating vs Sentiment Analysis
- Computed average rating per sentiment
- Identified **rating–sentiment misalignment**, including:
  - High rating with negative sentiment
  - Low rating with positive sentiment

This reveals **hidden dissatisfaction and emotional bias**.

---

### 6️⃣ Response Time Impact Analysis
- Average response time by sentiment
- Threshold-based sentiment distribution across response buckets
- Identifies **critical delays that escalate negative sentiment**

---

### 7️⃣ Complaint Behavior Analysis
- Complaint registration by sentiment
- Comparison between complaining vs non-complaining customers
- Helps detect **underreported dissatisfaction**

---

### 8️⃣ Issue Resolution Impact
- Sentiment comparison for resolved vs unresolved cases
- Strongly highlights the importance of **closure and resolution**

---

### 9️⃣ Comparative Performance Analysis
Sentiment analyzed across:
- Platforms
- Product categories
- Platform × Product combinations
- Regions (avg response time & rating)
- Age groups
- Gender

This enables **targeted operational improvements**.

---

### 🔟 Silent Dissatisfaction Detection
- Identified customers with **negative sentiment but no complaints**
- Quantified the percentage of silent dissatisfaction
- Critical for proactive customer retention strategies

---

### 1️⃣1️⃣ Custom Service Risk Score
A composite **Service Risk Score** was developed using:

- Response time (weighted)
- Unresolved issues
- Complaint registration

This score:
- Quantifies operational risk
- Flags high-risk customers
- Supports proactive intervention

---

## 📊 Visualization & Dashboard
The project includes:
- Multi-line trend visualizations
- Sentiment-based performance plots
- An integrated **Customer Sentiment & Service Experience Dashboard** showing:
  - Sentiment distribution
  - Ratings
  - Response time
  - Complaints
  - Issue resolution
  - Platform performance

The dashboard enables **executive-level decision-making**.

---

## 🔍 Key Insights
1. Positive sentiment customers receive faster responses and give higher ratings
2. Negative sentiment strongly correlates with delayed response and unresolved issues
3. Rating–sentiment misalignment reveals hidden dissatisfaction
4. A significant portion of dissatisfied customers remain silent
5. Certain platforms and product categories show elevated service risk
6. Issue resolution dramatically improves sentiment
7. Service risk scores peak for negative sentiment customers
8. Age groups differ in sensitivity to service delays
9. Complaint likelihood increases sharply as sentiment worsens
10. Service experience variables are tightly interconnected

---

## ✅ Business Recommendations
- Reduce response time, especially beyond **3–6 hours**
- Prioritize quick issue resolution
- Monitor silent dissatisfaction using sentiment signals
- Use service risk scores for early warnings
- Improve service quality on high-risk platforms/products
- Implement sentiment-aware customer support workflows
- Regularly monitor dashboards for bottleneck detection
- Audit rating–sentiment gaps to uncover service blind spots

---

## 🛠️ Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

---

## 📁 Project Structure (Suggested)

---

## 👤 Author
**Supratim Maity**  

---

⭐ *If you find this project valuable, consider starring the repository.*
