# Multi-store Retail Performance Analysis — Aurora Threads Boutique
<p align="center">
  <img src="assets/Overview.png" width="1000" />
</p>


---


## Business Overview
Aurora Threads is a premium fashion boutique specializing in high-end designer apparel, footwear, and accessories. Renowned for its curated collections and signature personalized shopping experience, the boutique operates three stores, catering to a discerning, fashion-forward clientele that values exclusivity and craftsmanship.

As competition intensifies in the luxury retail market, Aurora Threads is embracing data-driven decision-making to strengthen its strategic edge. With growing datasets capturing customer behavior, sales performance, product trends, and branch activity, the boutique now has the opportunity to uncover deeper insights in identifying top-performing categories, understanding high-value customer segments, and optimizing inventory allocation across locations. By leveraging these insights, Aurora Threads aims to refine its merchandising strategy, elevate customer engagement, and sustain its position as a leader in the luxury fashion space.


---


## Business Problem 
Aurora Threads is facing growing challenges in turning its expanding sales and customer data into meaningful insights. The boutique struggles to identify trends across product categories, track performance efficiently, and make timely, data-driven decisions. Without stronger analytical capabilities, key opportunities for optimizing inventory, improving customer engagement, and boosting sales performance are being missed.

**Key Problems**
1. Difficulty identifying category-level trends and shifting customer preferences
2. Inefficient performance tracking across branches and product lines
3. Limited visibility into product demand, leading to suboptimal inventory decisions
4. Lack of advanced analytics tools is slowing down decision-making
5. Missed opportunities to improve sales strategy and enhance customer experience


---


## Project Objectives

The objective of this project is to answer Aurora Threads’ most important business questions

1. Transform raw retail transaction data into a clear, intuitive, and insight-driven PowerBI dashboard

2. Analyze sales performance across products, customers, and store locations to answer key business questions

3. Identify patterns in customer behavior, product demand, and branch activity that impact revenue and growth

4. Enable interactive exploration through dynamic charts, filters, and slicers to support ad-hoc decision-making

5. Support data-driven decisions for inventory planning, product assortment, and merchandising strategy

6. Improve operational efficiency and business performance by replacing intuition-based decisions with actionable insights

7. Lay the foundation for a scalable, data-driven retail analytics model that supports sustainable growth and competitive advantage


---


## Data Dictionary
- **Date:** Date of the sale transaction
- **Store:** Store location
- **Product:** Product name or description
- **Category:** Product category (e.g., clothing, shoes, accessories)
- **Gender:** Gender of the target market for the product (e.g., male, female, unisex)
- **Quantity:**  Number of units sold
- **SalesAmount:** Sales amount for each product
- **CustomerID:** Unique identifier for each customer (for tracking repeat purchases and customer behavior)
- **Discount:** Discount applied to the transaction (if any)
- **PaymentType:** Payment method used for the transaction (e.g., cash, credit card, debit card,  online payment)


---


## Approach & Methodology
This project was developed entirely using **Microsoft PowerBI**, covering the full analytics workflow — from data cleaning and transformation to modeling, analysis, and visualization. The objective was to analyze customer behavior, churn risk, and portfolio insights using an integrated and interactive PowerBI dashboard solution.

**1. Data Cleaning & Transformation (Power BI Power Query)**
- Imported raw customer data into **Power BI** using Power Query Editor
- Performed data cleaning and transformation directly in Power BI:
  - Removed duplicates and filtered invalid or missing entries
  - Renamed columns and standardized field formats (e.g., text, numeric, dates)
  - Handled missing dates, prices, discounts, and units sold for transactions
  - Normalized CustomerID and transaction data.
  - Created **calculated columns** for:
    - `Customer Category` (Regular Spender, Mid Spender, High Spender)
    - `Quantity Category` (Low, Medium, High)
    - `Revenue`
  - Ensured consistency and data quality for downstream modeling

**2. DAX Measures (Power BI)**
- Created **custom DAX measures** to support key metrics and business logic, including:
  - `Total Quantity Sold`, `Total Customers`, `Total Revenue`, `Number of Stores`, etc
- Used **DAX functions** such as:
  - `CALCULATE`, `FILTER`, `DIVIDE`, `AVERAGEX`, `IF`, `VAR`, `COUNTROWS`, `DISTINCTCOUNT`, etc
- Applied calculated measures to support dynamic and filter-aware analysis across customer segments

**3. Interactive Visualization & Dashboard Design (Power BI)**

Developed a comprehensive suite of interactive dashboards using **Power BI Desktop**

**Visualization Techniques:**
- Used card visuals, bar/column charts, donut charts, a table, and filters/slicers
- Enabled interactive drill-downs by store

**4. Insight Generation & Business Alignment**
- Identified key customer behavior patterns
- Translated findings into **actionable business recommendations**


---

🔗 [View the Live Dashboard](https://app.powerbi.com/view?r=eyJrIjoiYTU1NTcxY2EtMTJjMy00ZDAwLWJiMmMtNjRkMWY3ODAyZDNkIiwidCI6ImZmMGYzZTNhLTNlNTMtNDU0Zi1iMmI1LTZjNjg3NTNiOGVlNCJ9)

## 🔢 STORE-LEVEL DEEP-DIVE ANALYSIS
Each store was analyzed individually to evaluate strengths, weaknesses, and improvement opportunities.

### Store-A Performance Analysis & Insight
<p align="center">
  <img src="assets/StoreA.png" width="1000" />
</p>

**1. Top KPIs (Key Performance Indicators)**
- Total Revenue: $83,268
- Total Quantity Sold: 264 Units
- Total Customers: 11

**2. Product Performance**
- Clothing leads sales with $63,828, followed by Accessories $19,440
- Top products include:
  - Sunglasses – $19K
  - Jumpsuit – $12K
  - Skirts – $8K
  
**3. Revenue Trend by Day**
- Peak days hit up to $19.4K (Day 4)
- Some days show performance dips below $3K, indicating fluctuating demand

**4. Customer Value**
- **CUST004** is the top customer, contributing $19,440 in revenue from 36 units, followed by **CUST025** with $12,150 from 27 units
- Revenue is highly concentrated, with a small number of customers accounting for a large share of total sales
- **CUST001** purchased a relatively high volume (30 units) but generated only $5,700 in revenue, indicating a lower average selling price and potential pricing or product-mix inefficiencies

**5. Payment Type**
- Online payments dominate with 47%
- Debit & credit card transactions make up the remaining majority (21% and 17% respectively)

**6. Gender Split**
- Female buyers represent 57% of total revenue, indicating stronger demand from women.

**Insights**
- Product sales are dominated by Women’s wear, such as jumpsuits, skirts, jackets, swimwear, and blouses, indicating a strong preference for premium female fashion.
- Store A experiences a higher share of digital payment methods, showing stronger adoption of modern checkout behavior.
- Customer purchases suggest a higher female customer base, with consistent spending patterns

**Business Interpretation**
- Strong potential for expansion of women’s premium collections.
- Promotions on complementary products (jewelry, handbags) would likely improve basket size.


### Store-B Performance Analysis & Insight
<p align="center">
  <img src="assets/StoreB.png" width="1000" />
</p>

**1. Key Metrics**
- Total Revenue: $104,958
- Total Quantity Sold: 258
- Total Customers: 10

**2. Product Category** 
- Accessories lead with $70,698, followed by Footwear with $27,270
- Clothing is lowest, contributing $6,990
Top Products are:
- Necklace – $21.6K
- Boots – $18.2K
- Ring – $15.0K
- Watch – $12.2K

**3. Sales Trend**
- Daily sales peak at $22K on Day 26 and are lowest on Day 5 with $3K. There is a fluctuation in the sales trend over the month, showing healthier revenue fluctuations compared to Store A

**4. Customer Value**
- Top customer “CUST026” contributed $21,600 with 36 units, representing a significant share

**5. Payment Type**
- Credit Card (35%) is the most used payment channel
- Cash (28%) comes second, then Online payment 26%

**6. Gender Split**
- Revenue is nearly balanced:
  - Female – 30%
  - Male – 29%
  - Unisex – 41%

**Insights**
- Store B generates stable but moderate performance across product lines
- Customers show a high affinity for accessories, indicating a strong focus on small fashion items and accessories
- Payment mix shows a higher share of credit card transactions, suggesting customers may be more price-conscious

**Business Interpretation**
- Campaigns such as “Buy More Save More” could help increase basket size
- Digital wallet or loyalty points could drive higher digital adoption



### Store-C Performance Analysis & Insight
<p align="center">
  <img src="assets/StoreC.png" width="1000" />
</p>

**1. Key Metrics**
- Total Revenue: $100,230
- Total Quantity Sold: 249 Units
- Total Customers: 10

**2. Product Category**
- Accessories are highest at $57,600
- Footwear accounts for $42,630
- Clothing is not significant

**3. Top Products**
- Handbags – $24K
- Loafers – $18K
- Sandals – $17K
- Wristwatch – $15K

**4. Sales Trend**
- Best day reaches $24K, with lower days dropping to $2K, the widest gap among stores.

**5. Customer Value**
- “CUST006” leads with $24,00 with 30 units, significantly above other buyers.

**6. Payment Type**
- Cash dominates at 46%
- Credit Card – 22%
- Online payments – 20.4%
**Interpretation:** Customers in Store C are more traditional in payment preference.

**7. Gender Split**
- The Majority of spending comes from Unisex products (58%)
- Female revenue is 24K (24%)
- Male contributions are lower

**Insights**
- Accessories and footwear contribute significantly to revenue.
- Customer traffic is more varied by demographic, possibly due to better store location or broader assortment.

**Business Interpretation**
- Increasing premium SKUs may yield strong returns.
- Seasonal campaigns could further maximize store footfall.


---


## Combined Overall Performance (All Stores)

**Key Consolidated Metrics** 
- Total Revenue: $288,456
- Total Quantity Sold: 771 units
- Total Customers: 31
- Number of Stores: 3

### **Revenue Overview**
**Top Product Category:**
- Accessories dominate with $147,738, accounting for over half of the total revenue

**High-Performing Products:**
- Handbags ($24K) and Necklaces ($22K) lead chain-wide

**Customer Contribution Patterns**
- Across all stores, revenue is concentrated among a few customers
- Top 1–5 customers account for over 33–40% of store sales
**This indicates:**
- High-value customers drive business.
- Customer loyalty or retention programs could be highly effective.

**Gender Revenue Breakdown**
- Unisex: $120.86K (42%)
- Female: $102.17K (35%)
- Male: $65.43K (23%)


---


## Cross-Store Comparison & Insights



**1. Revenue Comparison**
Store B leads in total revenue ($105K) despite selling fewer units (258) than Store A (264).
Store A moves the greatest volume, but at lower average price points.

**Overall,** Store B is the top contributor to profitability, though all stores add meaningful value.

**2. Payment Behavior Comparison**
- Store A: Strong online customer base (47%).
- Store B: Balanced mix across all payment channels.
- Store C: Cash is the preferred method (46%).

**Overall Insight:**
- Payment preferences differ by location. Increasing online payment adoption in Store C could improve conversion, while Store A may benefit from targeted in-store promotions.

**3. Gender Purchasing Behavior**
- Store A: Female shoppers make up the majority at 57%, generating revenue of $47.06K
- Store B: Unisex products attract the largest share of buyers (41%), with revenue of $43.34K
- Store C: Unisex items also draw the strongest customer segment (58%) of $58.08K in revenue
**Overall:** Unisex products represent the greatest market opportunity across the chain, while the male gender contributed the least

**4. Product Strategy Differences**
- Store A: Clothing is the primary revenue driver, generating $63,828
- Stores B and C: Accessories lead in total revenue.
**Chain-wide:** Accessories show the strongest growth and should remain a priority for stocking and marketing efforts.





















- Store A shows the highest product movement and customer patronage, indicating strong store traffic.

- Total Customers: 10,000
- Average Balance: $76,486
- Products per Customer: 1.53 on average
- Active Customers: 51.51%
- Median Credit Score: 652

### 📊 Customer Segmentation: Analysis & Insights
**1. By Location**
- France has 50% (5,014) of the total customers.
- Germany and Spain are almost equally represented (~25% each).

**2. By Age Group & Gender**
- Largest age segments:
   - 35–44: 3,981 customers
   - 25–34: 3,222 customers
- Younger segment (<25) is the smallest: only 457 customers
- Gender distribution is balanced across all age groups

**3. By Credit Score Band**
- Majority of customers have fair to poor credit:
   - Fair (580–669): 3,331 customers
   - Poor (<580): 2,362 customers
   - Good (670–739): 2,428 customers
- Only 655 customers have Excellent (800+) scores - just 6.5% of the base

**4. By Number of Products**
- Over 50% have only 1 product
  - 5,084 (1 product)
  - 4,590 (2 products)
- Very few are using 3+ products

**5. By Balance Band**
- High Balance (100k–150k): 3,830 customers
- Low Balance (<50k): 3,692 customers
- Medium (50k-100k): 1,509 customers
- Very High Balance (150k+): 969 customers
- Most balances are clustered at the extremes - either low or high, suggesting a bimodal distribution


### ⚠️ Key Challenges Identified
**1. Low Active Engagement**
- With only 51.51% active customers, nearly half of the customer base is disengaged or dormant.
  - This may contribute significantly to the 20.37% churn rate.

**2. Low Cross-Sell Penetration**
- Over 95% of customers have 1–2 products
  - Suggests missed opportunities for upselling/cross-selling additional financial services (loans, credit cards, investments, etc.)

**3. Weak Credit Quality**
- With a median credit score of 652 and 5,693 customers in Fair or Poor segments, the bank may be carrying higher credit risk.
  - Could impact loan default rates and profitability if not managed


---


## 📊 Churn & Risk Overview

<p align="right">
  <img src="assets/churn1.png" width="1000" />
</p>

### Top KPIs (Key Performance Indicators)
- Churn Rate: 20.37%
- No. of Customers churned: 2.037
- Churned Balance: $186M
- High-Risk Customers: 174
- High-Value Churn Rate: 24.98%
  - Key Risk: Nearly 25% of high-value customers churned, representing a significant financial loss and a priority focus area.

### 🌍 Churn by Location

| Country         | Churn Rate   | Churned Balance    | Key Insight                               |
|-----------------|--------------|--------------------|-------------------------------------------|
| **Germany**     |     32%      |       $97.9M       | Highest churn rate and balance loss       |
| **Spain**       |     17%      |       $29.9M       | Moderate churn, lower financial exposure  |
| **France**      |     16%      |       $57.7M       | Lower churn rate, but large value impact  |

⚠ Germany is a high-risk churn zone, both in terms of volume and financial value.

### Churn by Customer Type
**1. Active vs. Inactive**
- Inactive customers account for 65% of churn, which is only 48% of the base.
- Active customer churn rate = 35%, indicating even active users aren't fully engaged.

**Actionable Insight:** Inactivity is a major churn predictor. There is a need to consider stronger lifecycle management.

<p align="right">
  <img src="assets/risk2.png" width="1000" />
</p>

### Churn by Product Usage
| No. of Products    | Churn Rate    | No. of Churned     |
|--------------------|-------------- |--------------------|
|   1                |     28%       |        1,409       | 
|   2                |     8%        |        348         |
|   3                |     83%       |        220         | 
|   4                |     100%      |        60          |

Customers with only 1 product are the largest churn group (1,409 customers).

**Caution**

The dataset shows a 100% churn rate for customers with four products. On investigation, this segment has a very small sample size, and all instances are labelled as churned. This appears to be a dataset artifact rather than a realistic banking behavior, so insights from this segment should be interpreted with caution. Strategic focus should remain on 1–3 product customers, where both volume and churn impact are material.

### Churn by Age Group
| Age Group       | Churn Rate    | No. of Churned                        |
|-----------------|-------------- |---------------------------------------|
|   45-54         |     48%       |  Extremely high churn risk            |
|   55+           |     39%       |  Aging segment disengaging            |
|   35-44         |     18%       |  Moderate risk                        | 
|   <25           |     9%        |  Lower churn, oppourtunity to grow    |
|   25-34         |     8%        |   Best-performing segment             |

**Insight:** Mid-to-senior age customers are churning at 2-5x the rate of younger ones.

### Churn by Credit Score Band
| Credit Score Band       |  Churn Rate    |
|-------------------------|----------------|
|  Poor (<580)            |     22%        |
|  Fair (580-669)         |     21%        |
|  very Good (740-799)    |     21%        |
|  Excellent (800+)       |     20%        |
|  Good (670-739)         |     19%        |

**Insight:**

Churn is fairly consistent across credit bands, and no strong correlation between score and churn.

### Churn Balance by Risk Tier

| Risk Tier       |  Churned Balance  |
|-----------------|-------------------|
|  Medium         |     $106M         |
|  low            |     $79.4M        |
|  High           |     $0.2M         |

**Insight:**
- My analysis showed that customers at the highest churn risk tend to have lower balances, meaning they contribute less to direct financial loss.
- The majority of revenue loss actually comes from medium-risk, higher-value customers.
- This highlights the need for differentiated retention strategies.


---


## Financial Performance Summary

<p align="right">
  <img src="assets/Summary.png" width="1000" />
</p>

### KPIs Overview
- Total Customers: 10,000
- Churn Rate: 20.37% (2,037 customers churned)
- Average Retain Balance: $72,745
- Average Churn Balance: $91,109
- Total Balance: $765M
- Geographies: France, Germany, Spain

**Key Insights**
**1. High Churn Rate**
- A churn rate of 20.37% is relatively high, indicating a potential issue in customer retention.
- The average balance of churned customers ($91,109) is higher than that of retained customers ($72,745), suggesting that higher-value customers are churning.

**2. Geographical Distribution**
- Majority of customers are from:
  - France: 5,014 (50.1%)
  - Germany: 2,509 (25.1%)
  - Spain: 2,477 (24.8%)

However, a filtered drill-down shows:
- In Germany, customers under 25 years old, with medium churn risk, are notably present (96 customers).
- Within this filtered segment, gender is almost equally split: 41 males, 36 females.

**3. Age Group Analysis**
- Most customers fall into 35-44 and 25-34 age groups:
  - 35-44: 3,278 retained
  - 25-34: 2,972 retained

- However, <25 age group has the lowest retention (417) and churn (40) proportionally.
- Suggests younger customers are more likely to churn.

**4. Churn Risk Tiers**
- Within the Germany/<25/Medium Risk segment:
  - Most are in Medium Risk tier (77 out of 96).
  - Low (14) and High (5) are negligible.


---


## 🎯 Strategic Recommendations

A. **Customer Retention Strategy**

1. **Prioritize high-balance churners:**
   - Since churned customers have higher average balances, create retention campaigns targeting high-value customers.
   - Consider proactive outreach, loyalty rewards, or personalized financial advice.

2. **Develop targeted interventions for medium-risk segments:**
   - The largest risk category is medium. Launch "nudge" campaigns for this group to reduce the risk of escalation.
   - Examples: financial planning tools, regular check-ins, or premium service trials.

B. **Segment-Specific Strategies**

1. **Adults (45-54 age group) and Seniors (55+ age group)**
   - High churn and low retention indicate dissatisfaction or low engagement.
   - Actions:
     - Launch adults-focused products (e.g., retirement planning consultations, health savings-linked accounts, insurance bundles (health + life + critical illness)).
     - Improve digital engagement (mobile banking, in-app "easy mode" interface).

2. **Germany Segment**
   - Customers <25 in Germany are showing churn behavior.
   - Consider localized offers and customer engagement campaigns in Germany targeting this age group.

C. **Geographic Focus**
   - France has 50% of total customers – leverage this for upselling and cross-selling.
   - Spain and Germany: Evaluate marketing ROI and retention performance to determine if higher engagement is needed.

D. **Improve Churn Prediction & Early Warning**
   - Use the existing churn risk tiers to build a predictive churn model based on:
     - Age
     - Geography
     - Gender
     - Credit Score
     - Product usage
     - Balance trends
   - Focus on medium-risk segments and monitor any increase in early warning indicators.

E. **Financial Impact Monitoring**
   - Given that high churners have higher balances:
     - Quantify potential revenue loss from churn and build a business case for investing in retention programs.
     - Use dashboards to track CLV (Customer Lifetime Value) over time by segment.

### Next Steps

1. **Deep dive into churn drivers:** Survey churned customers, analyze product usage data.

2. **Build retention models:** Use machine learning (e.g., logistic regression, random forest) to predict churn risk.

3. **Refine segmentation:** Include behavioral data (transaction volume, complaints, digital activity).

4. **Test retention offers:** A/B test targeted campaigns for high-value and medium-risk customers.

5. **Monitor KPIs monthly:** Add trend charts for churn rate, NPS, and retention by geography and age.


---

🔗 [View the Live Dashboard](https://bit.ly/UnityBank_Customer_Churn_Risk)


## Executive Summary

This Power BI analytics solution provides Unity Bank with a comprehensive, data-driven view of its customer base, financial exposure, and churn risk. By leveraging the full capabilities of Power BI from data transformation to advanced DAX measures and interactive dashboards, the project delivers actionable insights that directly support customer retention, revenue protection, and risk mitigation efforts.

This analysis reveals that Unity Bank is facing a critical customer churn challenge, with over 20% of customers exiting and a disproportionately high churn among medium-risk and high-balance clients. Inactivity, low product penetration, and regional concentration (notably in Germany) emerge as leading indicators of churn. Additionally, the bank’s current churn risk tiering underestimates the risk posed by medium-tier customers, who account for the largest share of churned balance value.

The dashboards empower stakeholders to explore these dynamics through real-time, filterable views segmented by geography, age, credit score, product usage, and churn risk. This enables business leaders to move from reactive churn tracking to proactive customer engagement and risk prevention.

## Executive Recommendation

Unity Bank should implement a **targeted, data-driven customer retention strategy** focused on the following priorities:

1. **Prioritize Medium-Risk and High-Balance Customers**  
   - Proactively monitor and engage medium-risk customers, especially those with high balances, using early-warning signals from the dashboard.

2. **Reactivate Inactive Customers**  
   - Launch re-engagement campaigns and personalized offers for inactive users, who represent a large portion of churned customers.

3. **Increase Product Penetration to Reduce Churn**  
   - Design bundled product offerings and personalized cross-sell strategies to encourage customers with only one product to deepen their relationship with the bank.

4. **Localize Retention Strategies by Region**  
   - Tailor retention and service strategies for high-churn regions like Germany, where customer behavior significantly deviates from the rest of the portfolio.

5. **Refine Risk Scoring Models**  
   - Update churn risk models to reflect actual behavioral drivers found in the data, such as inactivity, single product ownership, and regional trends, to improve prediction accuracy.

By implementing these actions, Unity Bank can significantly reduce churn, improve customer lifetime value, and drive sustainable revenue growth through smarter, insight-led decisions.


---


## Disclaimer
This project is for portfolio and educational display only.

No content may be reused without permission.


---


## Connect With Me
- 💼 **LinkedIn:** (https://www.linkedin.com/in/david-okeleye001/)
- 📧 **Email:** okeleyedavid2021@gmail.com
- 🌐 **Portfolio:** https://bit.ly/3N5c1p7
- 🐙 **GitHub:** https://github.com/olavidz01-dev
