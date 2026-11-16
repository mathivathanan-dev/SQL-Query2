# BIKSERVICE – SQL Server Database Project

## Project Description
BIKSERVICE is a basic SQL Server database project developed to understand SQL queries, database creation, table creation, data insertion, data retrieval, and data type conversion using SQL Server Management Studio (SSMS).

## Technologies Used
- Microsoft SQL Server
- SQL Server Management Studio (SSMS)
- SQL

## Database Name
`BIKSERVICE`

## Tables

### 1. CUSTOMER

| Column Name | Data Type |
|---|---|
| CID | NUMERIC(3) |
| CNAME | VARCHAR(20) |
| PHONE | NUMERIC(13) |

### 2. OFFICE

| Column Name | Data Type |
|---|---|
| OID | INT |

## SQL Concepts Covered

1. CREATE DATABASE – Creating a database.
2. USE – Selecting a database.
3. CREATE TABLE – Creating tables.
4. INSERT INTO – Inserting records.
5. SELECT – Retrieving records.
6. DELETE – Deleting records.
7. DROP TABLE – Removing a table.
8. DROP DATABASE – Removing a database.
9. CAST() – Converting one data type into another.
10. CONCATENATION – Combining column values and strings.

## Sample SQL Queries

### Display Customer Records
```sql
SELECT * FROM CUSTOMER;
```

### Display Office Records
```sql
SELECT * FROM OFFICE;
```

### Insert Office Record
```sql
INSERT INTO OFFICE (OID)
VALUES (CAST('1' AS INT));
```

### CAST and Concatenation
```sql
SELECT CID,
       CNAME + '_' + CAST(CID AS VARCHAR(10))
FROM CUSTOMER;
```

## Expected Output

| CID | Result |
|---|---|
| 1 | GOKUL_1 |
| 2 | RAMESH_2 |
| 3 | PRAK
