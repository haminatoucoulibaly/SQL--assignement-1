# SQL--assignement# 🎤 Music World SQL Project

Welcome to my first SQL project — where **music meets data**! 🎶  
I built this for a class assignment, but it turned into a fun way to explore artists, cities, and countries through a simple relational database.

---

## 🌍 What's Inside

This mini music database includes:

- 🌐 **Countries** and their capitals  
- 🏙️ **Cities**  
- 🎤 **Artists** and their hometowns  

*(I removed the Genres table to keep things simple.)*

---

## 📚 What I Learned

- Creating tables with foreign key relationships  
- Inserting and updating data  
- Writing SQL queries with `SELECT`, `JOIN`, and filters  
- Fixing data issues (like the “Micheal” typo 😅)

---

## 🛠️ How to Use

1. Run `01_table_creation.sql` to create the tables  
2. Load sample data with `02_data_insertion.sql`  
3. Use the rest of the files to update and explore  
4. Try adding your favorite artist or city!

```sql
-- Example: Add your city!
INSERT INTO City (Id, City_name, Country_id)
VALUES (7, 'Your City', NULL);
-1
![SQL Assignement](https://github.com/user-attachments/assets/3a805773-9223-43bc-8d54-5e7164b97b4d)
