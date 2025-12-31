# Chinook Digital Media Store  

## 1. Background & Overview
Digital media platforms generate large volumes of transactional data from customer purchases, content catalogs, and employee operations. While transactional (OLTP) databases are effective for daily operations, they are not optimized for analytical queries such as customer behavior analysis, sales trends, or product performance evaluation.

This project uses the **Chinook Digital Media Store dataset** to demonstrate how sound **data modeling** and **data warehouse design** can transform raw transactional data into a structure optimized for analytics and business intelligence.

Rather than focusing on advanced machine learning, the project emphasizes:
- Relational data modeling principles  
- Referential integrity and business rules  
- Star and snowflake schema design  
- Business-driven analytical use cases  

**Core Business Question**  
> How can a transactional digital media database be transformed into a scalable data warehouse that supports efficient, insight-driven analytics?

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

<img width="1325" height="749" alt="image" src="https://github.com/user-attachments/assets/005563c8-fff7-49b4-8bcd-49656db94a15" />



