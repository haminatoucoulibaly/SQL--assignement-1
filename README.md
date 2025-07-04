# Relational SQL Practice Project

![Database Schema Diagram](assets/database_schema.png)
![SQL Assignement](https://github.com/user-attachments/assets/9dde2003-663f-4de0-9a50-fc5fe19b65ba)

*A visual overview of the tables and relationships*

---

## What's Inside?

This project features a simple, beginner-friendly relational SQL database designed to practice:

- Table creation with primary and foreign key relationships  
- Query writing (SELECT, JOIN, WHERE, etc.)  
- Data cleaning and updates  
- Schema design visualization

### Database Structure:

- **Countries** (`Country_id`, `Country_name`, `Country_Capital`, `Country_code`)
- **Cities** (`Id`, `City_name`, `Country_id`) → references `Countries`
- **People** (`Id`, `Name`, `City_id`, `Contact_Address`) → references `Cities`

> Note: A "Genres" table was originally part of the concept but has been removed for simplicity.

---

## How to Create This Diagram (If You Don't Have One)

You can use [DBML](https://dbdiagram.io/) to generate your own schema diagram.

### Example DBML Code:

```dbml
Table Country {
  Country_id integer [primary key]
  Country_name varchar [not null]
  Country_Capital varchar
  Country_code varchar(8)
}

Table City {
  Id integer [primary key]
  City_name varchar(128)
  Country_id integer [ref: > Country.Country_id]
}

Table Person {
  Id integer [primary key]
  Name varchar(128)
  City_id integer [ref: > City.Id]
  Contact_Address text
}


