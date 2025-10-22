# 🛫 Airline Database Analysis (SQL Project)

## 📘 Overview
The **AirlineDB** project focuses on exploring and analyzing an airline operations database to derive meaningful business insights using **SQL**.  
The dataset contains multiple interconnected tables related to **flights, tickets, bookings, boarding passes, and airports**, allowing the application of advanced SQL concepts such as joins, aggregations, subqueries, and window functions.  

This project demonstrates the ability to **query relational data, analyze operational efficiency, and present insights** that could support airline management decisions.

---

## 🎯 Objective
- To analyze airline operations data and uncover trends in **ticketing, flight volumes, and booking patterns**.  
- To apply **SQL querying techniques** to answer real-world business questions efficiently.  
- To practice **data cleaning, relationship handling, and analytical query building** within a relational database.  
- To demonstrate proficiency in **SQL joins, grouping, ranking, and date formatting**.  

---

## 🧰 Tools & Technologies Used
- **SQL** – For querying and analyzing relational datasets.  
- **PostgreSQL** (or compatible RDBMS) – As the database platform for executing SQL queries.  
- **Excel / Power BI** – (Optional) Used for visualization or summarizing query outputs.  
- **GitHub** – For version control and project documentation.  

---

## 🔍 Key Tasks & Queries
1. **Ticket Validation Analysis**  
   - Identified tickets that did not have corresponding boarding passes using `LEFT JOIN` and `NULL` filtering.  
   - Provided insights into operational gaps in ticket-to-pass linkage.

2. **Booking Trend Extraction**  
   - Extracted booking references, formatted booking dates (in `YYYY-MM-DD`), and total amounts from the `bookings` table.  
   - Applied the `TO_CHAR()` function to enhance readability and data presentation.

3. **Airport Ranking by Departures**  
   - Ranked airports based on total flight departures using `GROUP BY` and `RANK() OVER()` window functions.  
   - Provided insights into the busiest departure hubs in the dataset.

---

## 🧠 Concepts Demonstrated
- **Joins:** LEFT JOIN, INNER JOIN  
- **Aggregations:** COUNT, SUM, GROUP BY  
- **Filtering:** WHERE, HAVING  
- **Window Functions:** RANK(), DENSE_RANK()  
- **Date Formatting:** TO_CHAR(), DATE_TRUNC  
- **Data Cleaning:** Handling NULL values and duplicate entries  

---

## 📈 Key Insights
- Identified tickets missing boarding passes, indicating possible operational discrepancies.  
- Analyzed booking trends to understand transaction timelines and customer activity.  
- Ranked airports by departure frequency, offering visibility into flight distribution patterns.  

---

## 🚀 Outcomes
- Strengthened proficiency in **SQL-based data exploration and analysis**.  
- Developed a deeper understanding of **data relationships and real-world business queries**.  
- Built query-writing efficiency to support **data-driven decision-making** processes.  





