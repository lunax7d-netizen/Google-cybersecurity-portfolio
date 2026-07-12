-- Task 1: Match employees to their machines
SELECT * 
FROM machines 
INNER JOIN employees ON machines.device_id = employees.device_id;


-- Task 2: Return all machines and matching employees (LEFT JOIN)
SELECT * 
FROM machines 
LEFT JOIN employees ON machines.device_id = employees.device_id;


-- Task 2: Return all employees and matching machines (RIGHT JOIN)
SELECT * 
FROM machines 
RIGHT JOIN employees ON machines.device_id = employees.device_id;


-- Task 3: Retrieve login attempt data for employees
SELECT * 
FROM employees 
INNER JOIN log_in_attempts 
ON employees.username = log_in_attempts.username;
