# SQL-Airline-Database-Project
A SQL-based airline management system for analyzing flight, passenger, and revenue data

SQL Query Result – AirlineDB

**Question 1:** Find the number of tickets that do not have a corresponding boarding pass.

**SQL Query:**
```sql
select 
    count(*)
from tickets t
left join boarding_passes bp
    on t.ticket_no = bp.ticket_no
where bp.ticket_no is null;

**Question 2:** Retrieve the booking reference, booking date (in `yyyy-mm-dd` format), and total amount from the `bookings` table.

**SQL Query:**
```sql
select
    book_ref,
    to_char(book_date, 'yyyy-mm-dd') as book_date,
    total_amount
from bookings;


### 🟣 Database: AirlineDB
The **AirlineDB** is a database used as the basis for tutorials to teach SQL.  
The database contains flight-related data, including transactions, tickets, flights, airports, and flight schedules.

##**Question 3 **
Identify and rank the **departure airports** based on the **total number of flights** departing from each airport.  
The goal is to determine which airports handle the highest flight volumes.

---

### 💾 SQL Query:
```sql
SELECT
    departure_airport,
    COUNT(*) AS total_flights,
    RANK() OVER (ORDER BY COUNT(*) DESC) AS airport_rank
FROM flights
GROUP BY 1;

