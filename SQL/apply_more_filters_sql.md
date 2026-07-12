# Apply More Filters in SQL

## Objective

Use SQL filtering techniques to retrieve specific information from databases by applying comparison operators, the WHERE clause, and the BETWEEN operator to analyze dates, times, and numeric data.

## Scenario

As a security analyst, it is important to filter database information to quickly identify relevant security events. In this lab, SQL filters were used to investigate login attempts by date, time, and event ID to help analyze a potential security incident.

The information was retrieved from the organization database using the log_in_attempts table.

## Tools Used

- SQL
- MariaDB
- Linux Terminal
- SELECT
- FROM
- WHERE
- BETWEEN
- AND
- Comparison Operators (>, >=, <)

## Database Used

```sql
organization
```

## SQL Code

```sql
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
```

## Takeaways

- Learned how to filter SQL queries using the WHERE clause.
- Practiced using comparison operators to search for specific dates, times, and values.
- Used BETWEEN and AND to retrieve data within a specific range.
- Learned how filtering helps security analysts investigate login activity.
- Improved SQL skills for identifying suspicious events in large datasets.
