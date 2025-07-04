# Music World SQL Project

Welcome to my first SQL project — where music meets data.  
I created this as part of a class assignment, and it turned into a fun way to explore how artists, cities, and countries can be connected through a relational database.

---

## What's Inside

This project contains a simple SQL database with:

- Countries and their capitals  
- Cities around the world  
- Artists and their hometowns  

(Note: A Genres table was originally included but later removed to keep things simple.)

---

## What I Learned

- How to create tables with foreign key relationships  
- How to insert, update, and manage data  
- Writing SQL queries using SELECT, JOIN, and WHERE  
- Fixing data issues (e.g., typos like "Micheal")

---

## How to Use

1. Run `01_table_creation.sql` to set up the database schema  
2. Use `02_data_insertion.sql` to load sample data  
3. Continue with the remaining SQL files in order  
4. You can also customize the database by adding your own entries

```sql
-- Example: Add your own city
INSERT INTO City (Id, City_name, Country_id)
VALUES (7, 'Your City', NULL);
