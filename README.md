# SQL BMI Case Study (SQLBolt Lesson 3)

This repository contains a SQL practice project based on **SQLBolt – Lesson 3: Queries with Sorting & Limiting Results**, using a simple **BMI (Body Mass Index)** dataset.

## Description
This project focuses on retrieving and organizing data using `ORDER BY`, `LIMIT`, and `OFFSET`.  
The dataset includes user BMI and age data, which are sorted to find highest values, rankings, and specific positions in ordered results.

## Key Concepts (Lesson 3)
- `ORDER BY` for sorting query results
- Sorting with `ASC` and `DESC`
- Multi-column sorting (`ORDER BY column1, column2`)
- `LIMIT` to restrict number of rows returned
- `OFFSET` to skip rows in sorted results

## Example Queries
```sql
-- Get user with highest BMI
SELECT name, bmi
FROM user
ORDER BY bmi DESC
LIMIT 1;

-- Sort by BMI (highest first), then by age (youngest first)
SELECT name, bmi, age
FROM user
ORDER BY bmi DESC, age ASC;

-- Get the second highest BMI
SELECT name, bmi
FROM user
ORDER BY bmi DESC
LIMIT 1 OFFSET 1;

## Use Case
- Find users with the highest or lowest BMI
- Rank data based on multiple criteria
- Retrieve top-N or specific ranked records

## Tools
- SQL
- SQLite
- Visual Studio Code (SQLite Extension)

## File
- `bmi_lesson3.sql` – contains all Lesson 3 queries and examples

## Author
Zona Diatri
