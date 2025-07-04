# Music World SQL Project

This project combines music and data through a simple relational SQL database.  
It explores how countries, cities, and artists can be connected and queried using SQL.

---

## What's Inside

The database includes:

- Countries and their capitals  
- Cities around the world  
- Artists and their hometowns  

(Note: A Genres table was initially included but later removed to simplify the structure.)

---

## What I Learned

- Creating tables with foreign key relationships  
- Inserting, updating, and managing structured data  
- Writing queries using SELECT, JOIN, and WHERE clauses  
- Identifying and fixing data issues

---

## How to Use

1. Run `01_table_creation.sql` to create all tables  
2. Load sample data with `02_data_insertion.sql`  
3. Continue with the remaining SQL files to update and query the data  
4. Feel free to expand the dataset by adding your own entries

```sql
-- Example: Add your own city
INSERT INTO City (Id, City_name, Country_id)
VALUES (7, 'Your City', NULL);

