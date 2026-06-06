# Amazon Sales & Profit Analysis 📦

Hey! This project is a full data analytics case study on **50,000 Amazon orders** from 2022-2023. I wanted to understand what's really driving revenue, which regions perform best, and whether discounting actually works.

Built end-to-end - data cleaning, SQL queries, Python visualizations, and a Power BI dashboard.

---

## 📸 Dashboard Preview

![Amazon Sales Dashboard](Amazon%20Dashboard%20Image.png)

---

## What's This About?

I took a dataset of 50,000 orders across 6 product categories and 4 global regions, and asked real business questions:
- Which category makes the most money?
- Does higher discount = more sales?
- Which region has the most valuable customers?
- How does revenue trend month by month?

The answers surprised me in a few places.

---

## Files in This Repo

| File | What it is |
|---|---|
| [`Amazon Sales & Profit Analysis Dashboard.ipynb`](./Amazon%20Sales%20%26%20Profit%20Analysis%20Dashboard.ipynb) | Main notebook - cleaning, SQL, EDA, charts |
| [`amazon_sales.csv`](./amazon_sales.csv) | Raw dataset (50,000 rows) |
| [`Amazon_sales_dashboard.pbix`](./Amazon_sales_dashboard.pbix) | Power BI dashboard file |
| [`Amazon Dashboard Image.png`](./Amazon%20Dashboard%20Image.png) | Dashboard screenshot |

---

## Key Numbers

| Metric | Value |
|---|---|
| 💰 Total Revenue | $32.9 Million |
| 📈 Total Profit | $1.64 Million |
| 🛒 Total Orders | 50,000 |
| ⭐ Avg Rating | 3.0 / 5 |
| 🏷️ Avg Discount | 13.3% |

---

## Tools I Used

- **Python + Pandas** - data cleaning and exploration
- **SQLite + SQL** - answering business questions
- **Matplotlib + Seaborn** - visualizations
- **Power BI** - interactive dashboard
- **Jupyter Notebook** - putting it all together

---

## Project Phases

### Phase 1 - Data Cleaning
- Loaded 50,000 records with 14 columns
- Zero null values found ✅
- Engineered new columns: `discounted_price`, `total_revenue`, `profit`

---

### Phase 2 - Basic SQL (7 Questions)

| # | Question | Key Finding |
|---|---|---|
| Q1 | Highest revenue category? | Beauty leads |
| Q2 | Highest avg order value by region? | Middle East at $663 |
| Q3 | Most popular payment method? | Wallet with 10,106 orders |
| Q4 | Avg rating by category? | Home & Kitchen tops at 3.15 |
| Q5 | Highest avg discount? | Sports at 13.93% |
| Q6 | Total profit by region? | Middle East at $415K |
| Q7 | Highest quantity sold? | Beauty with 25,422 units |

---

### Phase 3 - Advanced SQL (5 Questions)

Used window functions, CTEs, subqueries, and running totals:

| # | Question | Technique |
|---|---|---|
| Q1 | Above-average revenue orders per category | Subquery |
| Q2 | Rank categories by total profit | `RANK()` |
| Q3 | Top 5 revenue orders per region | `ROW_NUMBER()` |
| Q4 | Running total of revenue | `SUM() OVER()` |
| Q5 | High discount + low rating products | Conditional filter |

---

### Phase 4 - Visualizations

**Python charts:**
- Revenue by Category - Bar Chart
- Avg Order Value by Region - Bar Chart
- Payment Method Distribution - Pie Chart
- Avg Discount by Category - Bar Chart
- Region × Category Revenue - Heatmap

**Power BI Dashboard:**
- Monthly Revenue Trend (2022-2023)
- Revenue by Region
- Revenue by Category (Donut)
- Payment Method Distribution (Donut)
- Interactive Year & Month slicers

---

## What I Found - Key Insights

**1. Beauty dominates volume, but Middle East dominates value**
Beauty has the most orders, but the Middle East region has the highest average order value ($663) and total profit. Premium market = premium returns.

**2. High discounts aren't fixing low ratings**
Sports category has the highest discount (13.93%) but ratings are still around 3.0. Discounting alone doesn't fix a product problem.

**3. Payment methods are evenly distributed**
No single payment method dominates - Wallet, UPI, COD, Credit & Debit Card all perform similarly. Good sign for platform flexibility.

**4. Revenue is surprisingly stable month-to-month**
The monthly trend stays between $2.6M-$2.8M with a February spike - suggesting steady demand rather than seasonal spikes.

**5. Overall rating of 3.0/5 is a red flag**
Consistent across all categories - points to a platform-wide issue with either product quality or delivery experience.

---

## My Recommendations

- Double down on the **Middle East** region - highest value customers, highest profit margin
- Fix the **rating problem** before pushing more discounts - customers aren't happy
- Investigate the **February spike** - if it's repeatable, it's a marketing opportunity
- **Sports category** needs a product quality review, not a bigger discount

---

## Let's Connect

Always happy to talk data, get feedback, or collaborate!

- 🐙 GitHub: [github.com/jiveshhmishra](https://github.com/jiveshhmishra)
- 💼 LinkedIn: [linkedin.com/in/jiveshh](https://www.linkedin.com/in/jiveshh/)
- 🔗 Portfolio: [https://jivesh.carrd.co/)

---

*Made with Python, SQL & Power BI · 2026*

