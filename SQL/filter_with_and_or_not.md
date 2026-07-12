# Filter with AND, OR, and NOT

## Objective

Use SQL operators such as AND, OR, and NOT to create more advanced filters, retrieve specific information from databases, and analyze security-related data more efficiently.

## Scenario

As a security analyst, it is important to filter database information using multiple conditions to find specific records. In this lab, SQL filters were used to investigate failed login attempts, identify login activity from specific locations, and retrieve employee information based on departments and office locations.

The information was retrieved from the organization database using the log_in_attempts and employees tables.

## Tools Used

- SQL
- MariaDB
- Linux Terminal
- SELECT
- FROM
- WHERE
- AND
- OR
- NOT
- LIKE

## Database Used

```sql
organization
```

## SQL Code

```sql
-- Task 1: Retrieve after hours failed login attempts
SELECT *
FROM log_in_attempts
WHERE login_time > '18:00:00' AND success = 0;


-- Task 2: Retrieve login attempts on specific dates
SELECT *
FROM log_in_attempts
WHERE login_date = '2022-05-09' OR login_date = '2022-05-08';


-- Task 3: Retrieve login attempts outside of Mexico
SELECT *
FROM log_in_attempts
WHERE NOT country LIKE 'MEX%';


-- Task 4: Retrieve employees in Marketing department in East building
SELECT *
FROM employees
WHERE department = 'Marketing' AND office LIKE 'East%';


-- Task 5: Retrieve employees in Finance or Sales departments
SELECT *
FROM employees
WHERE department = 'Finance' OR department = 'Sales';


-- Task 6: Retrieve employees not in Information Technology department
SELECT *
FROM employees
WHERE NOT department = 'Information Technology';
```

## Takeaways

- Learned how to use AND, OR, and NOT operators to create advanced SQL filters.
- Practiced combining multiple conditions to retrieve specific records.
- Used the LIKE operator to search for matching text patterns.
- Learned how SQL filtering can help security analysts investigate login activity and employee information.
- Improved SQL query skills for identifying security-related data in databases.
