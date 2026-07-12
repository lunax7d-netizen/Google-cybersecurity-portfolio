# Filter a SQL Query

## Overview
This lab practiced filtering SQL queries to retrieve specific information from a database.

Database used:
- organization

Tables used:
- machines
- employees

Commands and concepts practiced:
- SELECT
- FROM
- WHERE
- LIKE
- DESCRIBE

---

# Orientation: Know Your Data

## View table structures

```sql
DESCRIBE machines;

DESCRIBE employees;
```

Purpose:
- Shows columns and data types in a table.

---

# Task 1: List All Organization Machines

## Retrieve device IDs and operating systems

```sql
SELECT device_id, operating_system
FROM machines;
```

Result:
- Rows returned: 200

---

# Task 2: Retrieve Machines Using OS 2

## Filter machines by operating system

```sql
SELECT device_id, operating_system
FROM machines
WHERE operating_system = 'OS 2';
```

Result:
- Machines using OS 2: 88

---

# Task 3: List Employees in Specific Departments

## Find employees in Finance

```sql
SELECT *
FROM employees
WHERE department = 'Finance';
```

Result:
- First employee ID: 1049

## Find employees in Sales

```sql
SELECT *
FROM employees
WHERE department = 'Sales';
```

Result:
- Employees in Sales department: 33

---

# Task 4: Identify Employee Machines

## Find employee using South-109

```sql
SELECT *
FROM employees
WHERE office = 'South-109';
```

Result:
- Employee: jlansky

## Find all employees in the South building

```sql
SELECT *
FROM employees
WHERE office LIKE 'South%';
```

Result:
- First employee department: Sales

---

# SQL Commands Learned

| Command | Purpose |
|---|---|
| SELECT | Chooses columns to display |
| FROM | Chooses the table |
| WHERE | Filters results |
| LIKE | Searches for patterns |
| % | Wildcard for matching text |
| DESCRIBE | Shows table structure |

---

# Skills Practiced

- Filtering SQL queries
- Searching specific records
- Using WHERE conditions
- Using LIKE for pattern matching
- Understanding database tables
