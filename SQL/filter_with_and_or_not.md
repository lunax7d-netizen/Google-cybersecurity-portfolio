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
