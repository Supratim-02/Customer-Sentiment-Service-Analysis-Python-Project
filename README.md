# Customer Sentiment & Service Experience Analysis

## 📌 Project Overview
This project presents an **end-to-end customer sentiment and service experience analysis** using Python.  
It combines data cleaning, exploratory analysis, statistical summarization, custom risk modeling, and visual dashboards to uncover actionable insights that help improve **customer support performance and service quality**.

The analysis focuses on understanding how **sentiment, ratings, response time, complaints, and issue resolution** interact and influence customer satisfaction.

---

## 🎯 Project Objectives
- Analyze the overall distribution of customer sentiment (positive, neutral, negative)
- Examine alignment and misalignment between customer ratings and expressed sentiment
- Evaluate the impact of response time on customer sentiment
- Study how complaint registration and issue resolution affect satisfaction
- Identify **silent dissatisfied customers** who did not raise complaints
- Compare sentiment across platforms, product categories, regions, age groups, and gender
- Build a **service risk score** to quantify operational risk
- Create a **visual dashboard** connecting sentiment, ratings, response time, complaints, and resolution
- Derive data-driven recommendations for customer support optimization

---

## ❓ Business & Analytical Questions
This project answers questions such as:
- What is the overall sentiment distribution of customers?
- Do customer ratings always reflect sentiment?
- How does response time influence negative sentiment?
- Which response-time thresholds increase dissatisfaction?
- Are unresolved issues linked to negative sentiment?
- Are there dissatisfied customers who never file complaints?
- Which platforms and product categories show higher service risk?
- How does sentiment vary across demographics and regions?
- How can service risk be quantified numerically?

---

## 🧠 Analytical Approach
### 1. Data Loading & Exploration
- Dataset imported using **Pandas**
- Structure and summary explored using `info()` and `describe()`

### 2. Data Cleaning & Standardization
- Handled missing categorical values
- Standardized text columns (lowercase, trimmed)
- Normalized binary fields (`issue_resolved`, `complaint_registered`)
- Removed duplicate records

### 3. Feature Engineering
- Created `review_length` to measure customer feedback depth
- Bucketed response time into meaningful intervals (`<1h`, `1–3h`, `3–6h`, etc.)

### 4. Sentiment & Rating Analysis
- Sentiment distribution and percentage contribution
- Average customer rating by sentiment
- Identified **rating–sentiment misalignment** cases

### 5. Service Performance Analysis
- Response time analysis by sentiment
- Threshold-based response time impact
- Complaint registration patterns
- Issue resolution vs sentiment comparison

### 6. Comparative Analysis
- Platform-wise sentiment performance
- Product category sentiment comparison
- Platform × Product × Sentiment analysis
- Demographic analysis (age group, gender)
- Regional response time and rating performance

### 7. Silent Dissatisfaction Detection
- Identified customers with negative sentiment who did not register complaints

### 8. Custom Service Risk Score
A composite score built using:
- Response time
- Issue resolution status
- Complaint registration

This score helps flag **high-risk service cases** proactively.

---

## 📊 Visualizations & Dashboard
- Multi-line plots for platform-wise response time by sentiment
- Age-group sensitivity analysis for ratings
- A **comprehensive dashboard** visualizing:
  - Sentiment distribution
  - Average ratings
  - Response time trends
  - Complaint behavior
  - Issue resolution share
  - Platform-wise service performance

---

## 🔍 Key Insights
- Positive sentiment customers receive faster responses and give higher ratings
- Negative sentiment is strongly linked to delayed response and unresolved issues
- Rating–sentiment misalignment reveals hidden dissatisfaction
- A significant portion of negative customers never file complaints
- Certain platforms and product categories carry higher service risk
- Unresolved issues dramatically increase negative sentiment
- Service risk score is highest among negative sentiment customers
- Age groups show different sensitivity to service delays
- Complaint registration increases sharply as sentiment turns negative

---

## ✅ Recommendations
- Reduce response times, especially beyond the **3–6 hour threshold**
- Prioritize quick issue resolution to prevent sentiment escalation
- Monitor silent dissatisfied customers using sentiment signals
- Use service risk scores for proactive customer intervention
- Improve support quality on high-risk platforms and products
- Implement sentiment-aware customer support routing
- Track dashboards regularly to identify operational bottlenecks
- Review rating–sentiment mismatches to uncover hidden service gaps

---

## 🛠️ Tools & Technologies
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- Jupyter Notebook

---
