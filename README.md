# A/B Testing: Comparison of Bidding Strategies

## 📌 Project Overview
In this project, the impact of **Maximum Bidding** and **Average Bidding** strategies used in
Facebook advertising campaigns is analyzed through an **A/B test**.

The main objective is to determine whether the newly introduced *Average Bidding* strategy
leads to a statistically significant increase in purchases compared to the existing
*Maximum Bidding* strategy.

---

## 📊 Dataset
The dataset contains advertising performance metrics of an e-commerce company.

**Variables:**
- **Impression:** Number of ad impressions  
- **Click:** Number of ad clicks  
- **Purchase:** Number of purchases after clicks  
- **Earning:** Revenue generated from purchases  

The data consists of two experimental groups:
- **Control Group:** Maximum Bidding
- **Test Group:** Average Bidding

---

## 🧪 A/B Testing Process

1. **Hypothesis Definition**
   - H₀: There is no difference between the average purchases of the control and test groups.
   - H₁: There is a significant difference between the average purchases of the control and test groups.

2. **Assumption Checks**
   - Normality assumption → *Shapiro-Wilk Test*
   - Homogeneity of variances → *Levene Test*

3. **Test Selection**
   - Since both assumptions are satisfied, an **Independent Two-Sample T-Test** is applied.

4. **Result Interpretation**
   - The obtained p-value is greater than 0.05, therefore the null hypothesis cannot be rejected.

---

## 📈 Results and Business Insights
The analysis shows that the **Average Bidding** strategy does not provide a statistically
significant improvement in purchase conversions compared to the **Maximum Bidding** strategy.

🔎 **Business Recommendation:**
Based on the test results, it is recommended that the company continues using the current
bidding strategy, as switching to Average Bidding does not yield a measurable advantage.

---

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- SciPy
- Statsmodels
