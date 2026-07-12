# Complete a SQL Join

## Objective

Use SQL joins to combine information from multiple database tables, retrieve related data, and analyze relationships between employees, machines, and login activity.

## Scenario

As a security analyst, it is important to know how to retrieve and connect information stored across different database tables. In this lab, SQL joins were used to investigate a security incident by matching employees with their assigned machines and analyzing login activity.

The information was retrieved from the organization database using the machines, employees, and log_in_attempts tables.

## Tools Used

- SQL
- MariaDB
- Linux Terminal
- SELECT
- FROM
- ON
- INNER JOIN
- LEFT JOIN
- RIGHT JOIN

## Database Used

```sql
organization
```

## SQL Code

```sql
-- Task 1: Match employees to their machines
SELECT * 
FROM machines 
INNER JOIN employees 
ON machines.device_id = employees.device_id;

-- Task 2: Return all machines and matching employees (LEFT JOIN)
SELECT * 
FROM machines 
LEFT JOIN employees 
ON machines.device_id = employees.device_id;

-- Task 3: Return all employees and matching machines (RIGHT JOIN)
SELECT * 
FROM machines 
RIGHT JOIN employees 
ON machines.device_id = employees.device_id;

-- Task 4: Retrieve login attempt data for employees
SELECT * 
FROM employees 
INNER JOIN log_in_attempts 
ON employees.username = log_in_attempts.username;
```

## Takeaways

- Learned how to combine multiple database tables using SQL joins.
- Practiced using INNER JOIN, LEFT JOIN, and RIGHT JOIN.
- Learned how shared columns like `device_id` and `username` connect tables.
- Used SQL joins to investigate employee devices and login activity.
- Improved skills in retrieving and analyzing security-related data from databases.
