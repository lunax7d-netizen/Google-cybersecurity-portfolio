-- Task 1: Match employees to their machines using INNER JOIN

SELECT *
FROM machines
INNER JOIN employees
ON machines.device_id = employees.device_id;


-- Task 2: Return all machines and assigned employees using LEFT JOIN

SELECT *
FROM machines
LEFT JOIN employees
ON machines.device_id = employees.device_id;


-- Return all employees and assigned machines using RIGHT JOIN

SELECT *
FROM machines
RIGHT JOIN employees
ON machines.device_id = employees.device_id;


-- Task 3: Retrieve login attempt data using INNER JOIN

SELECT *
FROM employees
INNER JOIN log_in_attempts
ON employees.username = log_in_attempts.username;
