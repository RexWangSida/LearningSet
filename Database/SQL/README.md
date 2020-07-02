# SQL(Structured Query Language)
- descriptive words
- non-procedural language

## Data Retrieval
- **Using `SELECT` (columns) and `FROM` (table)**
- Table Example: Products
  | prod_name | prod_id | prod_price |
  |-----------|---------|------------|
  | Shampoo   |P01      | 12         |
  |Toothpaste |P02      | 13         |
  |Deodorant  |P03      | 20         |
  |Toothbrush |P04      | 5          |
```sql
/* retrive the column of prod_name */
SELECT prod_name
FROM Products;
```
```sql
/* retrive the columns of prod_name, prod_id */
SELECT prod_name, prod_id
FROM Products;
```

```sql
/* retrive the all columns */
SELECT *
FROM Products;
```
## Table Creation
- **Using `CREATE TABLE` to create table**
- Built-in Types:
  - **INT** or **INTEGER**
  - **FLOAT** or **REAL**
  - **CHAR(n)**
```sql
CREATE TABLE Student(
    SID CHAR(8),
    Name CHAR(20),
    Email CHAR(20),
    Age INTEGER,
    GPA REAL
);
```
- Setting **primary key** and **NULL/NOT NULL**
```sql
CREATE TABLE Student(
    SID CHAR(8) PRIMARY KEY,
    Name CHAR(20) NOT NULL,
    Email CHAR(20) NOT NULL,
    Age INTEGER NOT NULL,
    GPA REAL NULL
);
```

## Data Record Insertion
- **Using `INSERT INTO` and `VALUES` to create table**
- Table Example: Products
  | prod_name | prod_id | prod_price |
  |-----------|---------|------------|
  | Shampoo   |P01      | 12         |
  |Toothpaste |P02      | 13         |
  |Deodorant  |P03      | 20         |
  |Toothbrush |P04      | 5          |
```sql
/* insert with all values of all columns*/
INSERT INTO Products
VALUES (
  'sugar',
  'P05',
  3
);
```