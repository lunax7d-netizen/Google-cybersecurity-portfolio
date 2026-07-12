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
-- Match employees to their machines
SELECT * 
FROM machines 
INNER JOIN employees 
ON machines.device_id = employees.device_id;


-- Return all machines and assigned employees
SELECT * 
FROM machines 
LEFT JOIN employees 
ON machines.device_id = employees.device_id;


-- Return all employees and assigned machines
SELECT * 
FROM machines 
RIGHT JOIN employees 
ON machines.device_id = employees.device_id;


-- Retrieve login attempt data
SELECT * 
FROM employees 
INNER JOIN log_in_attempts 
ON employees.username = log_in_attempts.username;
```

## Results

- The INNER JOIN between machines and employees returned 185 rows.
- The LEFT JOIN showed all machines, including machines without assigned employees.
- The RIGHT JOIN showed all employees, including employees without assigned machines.
- The INNER JOIN between employees and log_in_attempts returned 200 records.

## Takeaways

- Learned how SQL joins connect information stored across multiple tables.
- Practiced using INNER JOIN to retrieve matching records.
- Used LEFT JOIN and RIGHT JOIN to identify missing relationships between tables.
- Learned how shared columns such as device_id and username connect database tables.
- Applied SQL joins to investigate cybersecurity incidents involving employee devices and login activity.
