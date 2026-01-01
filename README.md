# 💿 Chinook Digital Media Store  

## 1. Background & Overview
Digital media platforms generate large volumes of transactional data from customer purchases, content catalogs, and employee operations. While transactional (OLTP) databases are effective for daily operations, they are not optimized for analytical queries such as customer behavior analysis, sales trends, or product performance evaluation.

This project uses the **Chinook Digital Media Store dataset** to demonstrate how sound **data modeling** and **data warehouse design** can transform raw transactional data into a structure optimized for analytics and business intelligence.

Rather than focusing on advanced machine learning, the project emphasizes:
- Relational data modeling principles  
- Referential integrity and business rules  
- Star and snowflake schema design  
- Business-driven analytical use cases  

---

## 2. Data Structure & Initial Checks

The Chinook dataset represents a digital media store, including customer purchases, employee operations, and media content such as artists, albums, and tracks. The ER diagram highlights the relational structure that supports transactional integrity and business rules.

<img width="542" height="496" alt="image" src="https://github.com/user-attachments/assets/fe6295f9-3596-463d-a54e-a31d158694cf" />

The ER diagram highlights key one-to-many and many-to-many relationships enforced through primary and foreign keys to support transactional integrity.

[View business rules](https://github.com/kietngwork/chinook-database-design/blob/main/Chinook%20Business%20Rules.pdf)

---

## 3. Executive Summary

**Overview of Findings**

Overall performance is strong, with total sales of **2.3K** driven by **412 orders** from **59 customers**, reflecting healthy engagement and ~**24% period-over-period growth**. Growth is primarily fueled by higher order frequency rather than increased spend per order, with sales concentrated in the **U.S. market** and a heavy reliance on **MPEG audio** as the dominant media format.

Below is the overview page from the Power BI dashboard, with additional examples included throughout the report. The entire interactive dashboard can be downloaded [here](https://github.com/kietngwork/chinook-sales-dashboard/blob/main/Chinook%20Dashboard.pbix).

<img width="1278" height="723" alt="image" src="https://github.com/user-attachments/assets/41e008e4-44c9-4571-a45f-4521aabf2f4e" />


**Sales Trends:**
- **Sales remain relatively stable over time**, indicating a mature and predictable revenue pattern rather than volatility.
- A **clear peak around 2010** sets a high comparison base, leading to **normalized growth** in later years.
- **Mid-year months (June–August)** consistently outperform, suggesting **seasonal demand strength** during this period.
- A **dip toward November** followed by a **mild December recovery** points to **short-term seasonal softness rather than structural decline**.
- Growth is **driven primarily by order volume**, not higher spend per order, highlighting opportunities to **optimize Average Order Value**.

<img width="668" height="261" alt="image" src="https://github.com/user-attachments/assets/db958fc7-df4b-4ae8-9b0c-a931f846a87d" />


**Market Performance:**
- **The United States is the dominant market**, contributing the majority of total sales and orders, making it the primary growth driver but also a concentration risk.
- **Canada and France** follow as secondary markets, providing steady contributions but at significantly lower scale.
- Several smaller markets show **lower order counts but higher AOV**, suggesting opportunities for **targeted pricing, bundling, or niche-focused strategies**.
- Overall market performance reflects a **strong core market supported by long-tail international demand**, where growth potential lies in optimization rather than broad expansion.

<img width="660" height="269" alt="image" src="https://github.com/user-attachments/assets/08160a7a-35b3-4c7c-8581-761ed5643f60" />

**Recommendations:**
Based on the uncovered insights, the following recommendations have been provided:
### Recommendations (Data-Driven)

- **Increase Average Order Value (AOV)**, as total sales of **2.3K** are driven by **412 orders** rather than higher spend per transaction, with AOV currently at **5.7**.
- **Reduce reliance on the U.S. market**, which contributes the largest share of total sales, by scaling proven offerings in **Canada and France**, which together account for a meaningful share of total orders.
- **Exploit peak seasonality**, as sales perform strongest during **June–August**, by scheduling major campaigns and releases in this period.
- **Offset late-year softness**, particularly in **November**, where sales dip before recovering in **December**, through targeted discounts or bundled offers.
- **Diversify the media mix**, as **MPEG audio represents ~84% of total sales**, creating concentration risk in format dependency.
- **Leverage high-AOV niches**, where certain countries and genres generate fewer orders but higher revenue per order, indicating potential for premium pricing.
- **Sustain operational stability**, since items per order and average net sales remain consistent across months, supporting low-risk optimization initiatives.





