# Linux Grep and Filtering

## Objective

Use Linux commands such as `grep` and piping to search files, filter information, and locate specific data within system files.

## Scenario

As part of a cybersecurity lab, I practiced using Linux filtering tools to search through log files and user data files. These skills are important for security analysts when investigating system events, reviewing logs, and finding specific information efficiently.

## Tools Used

- Linux
- Bash
- grep
- Pipe operator (`|`)

## Commands Used

### Navigate to Log Directory

```bash
cd /home/analyst/logs
```

### Search for Error Messages in Logs

```bash
grep error server_logs.txt
```

### Navigate to User Reports Directory

```bash
cd /home/analyst/reports/users
```

### Filter Files Containing Specific Strings

```bash
ls | grep Q1
```

### Search for Files Containing Access Information

```bash
ls | grep access
```

### Search File Contents for a Username

```bash
grep jhill Q2_deleted_users.txt
```

### Search for Users in a Specific Department

```bash
grep "Human Resources" Q4_added_users.txt
```

## Skills Demonstrated

- Linux Command Line Filtering
- Log File Analysis
- Searching Files with grep
- Using Pipes for Data Filtering
- User Data Investigation
- Cybersecurity Log Analysis

## Key Takeaways

- Used `grep` to search for specific strings inside files.
- Used the pipe operator (`|`) to pass command output into another command.
- Filtered log files to identify error messages.
- Located files based on specific naming patterns.
- Searched user records for relevant security information.

## Outcome

Successfully used Linux filtering commands to analyze log files, search user data, and extract specific information. This lab improved my ability to investigate and process data using the Linux command line.
