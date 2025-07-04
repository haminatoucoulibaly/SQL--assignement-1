# Music World SQL Project

![Database Schema Diagram](assets/database_schema.png)
![SQL Assignement](https://github.com/user-attachments/assets/bb3586e6-668a-490b-a46d-1a2d0a2395a2)

*A visual overview of the tables and their relationships*

---

## What's Inside

This project includes a simple relational SQL database with:

- **Countries**  
  Columns: `id`, `name`, `capital`, `code`

- **Cities**  
  Columns: `id`, `name`, `country_id`  
  → Foreign key referencing `Countries.id`

- **Artists**  
  Columns: `id`, `name`, `city_id`, `contact_address`  
  → Foreign key referencing `Cities.id`

- ~~Genres~~ (removed in Question 6 to simplify the model)

---

## How to Create This Diagram (If You Don’t Have One Yet)

You can generate a database diagram using [DBML](https://dbml.dbdiagram.io/home) (Database Markup Language):

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

Table Artist {
  Artist_id integer [primary key]
  Artist_name varchar(128)
  City_id integer [ref: > City.Id]
  Contact_Address text
}

