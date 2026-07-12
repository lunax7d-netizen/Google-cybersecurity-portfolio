# Perform a SQL Query

## Overview
This lab practiced using basic SQL queries to retrieve and organize information from a database. The main commands used were SELECT, FROM, and ORDER BY.

Database used:
- organization

Tables used:
- machines
- log_in_attempts

---

# Task 1: Retrieve Employee Device Data

## View all information from machines table

```sql
SELECT *
FROM machines;
```

## Select specific columns

```sql
SELECT device_id, email_client
FROM machines;
```

Result:
- Third row email client: Email Client 2

## Select device information and patch dates

```sql
SELECT device_id, operating_system, OS_patch_date
FROM machines;
```

Result:
- First patch date: 2021-09-01

---

# Task 2: Investigate Login Activity

## Select event IDs and countries

```sql
SELECT event_id, country
FROM log_in_attempts;
```

Result:
- No login attempts were made from Australia.

## View usernames and login times

```sql
SELECT username, login_date, login_time
FROM log_in_attempts;
```

Result:
- Fifth row username: jrafael

## View all login attempts

```sql
SELECT *
FROM log_in_attempts;
```

---

# Task 3: Order Login Attempts Data

## Sort login attempts by date

```sql
SELECT *
FROM log_in_attempts
ORDER BY login_date;
```

Result:
- First record:
  - Username: ivelasco
  - Date: 2022-05-08

## Sort by date and time

```sql
SELECT *
FROM log_in_attempts
ORDER BY login_date, login_time;
```

Result:
- First record:
  - Username: bsand
  - Login time: 00:19:11

---

# Commands Learned

| Command | Purpose |
|---|---|
| SELECT | Chooses columns to display |
| FROM | Chooses the table to retrieve data from |
| * | Selects all columns |
| ORDER BY | Sorts query results |

---

# Skills Practiced

- Retrieving data from SQL tables
- Selecting specific columns
- Viewing complete tables
- Sorting database results
- Analyzing security-related login information
