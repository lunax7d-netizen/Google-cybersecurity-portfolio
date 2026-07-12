-- Task 1: Login attempts after a certain date
SELECT *
FROM log_in_attempts
WHERE login_date > '2022-05-09';

-- Login attempts on or after a certain date
SELECT *
FROM log_in_attempts
WHERE login_date >= '2022-05-09';


-- Task 2: Login attempts within a date range
SELECT *
FROM log_in_attempts
WHERE login_date BETWEEN '2022-05-09' AND '2022-05-11';


-- Task 3: Login attempts before working hours
SELECT *
FROM log_in_attempts
WHERE login_time < '07:00:00';


-- Login attempts between specific times
SELECT *
FROM log_in_attempts
WHERE login_time BETWEEN '06:00:00' AND '07:00:00';


-- Task 4: Login attempts by event ID
SELECT event_id, username, login_date
FROM log_in_attempts
WHERE event_id >= 100;


-- Event IDs between 100 and 150
SELECT event_id, username, login_date
FROM log_in_attempts
WHERE event_id BETWEEN 100 AND 150;
