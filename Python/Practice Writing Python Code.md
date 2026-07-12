# Practice Writing Python Code

## Objective

Use Python to write basic programs, understand Python syntax, work with variables, data types, conditional statements, and loops to automate cybersecurity-related tasks.

## Scenario

As a security analyst, Python can be used to automate repetitive tasks, analyze data, and improve security workflows. In this lab, Python code was written and tested to practice fundamental programming concepts that are commonly used in cybersecurity automation.

## Tools Used

- Python
- Jupyter Notebook
- Google Colab
- Variables
- Data Types
- Conditional Statements
- Loops
- Print Statements

## Python Code

```python
# Task 1: Create and display variables

username = "analyst"
login_attempts = 5
account_locked = False

print(username)
print(login_attempts)
print(account_locked)


# Task 2: Use conditional statements

failed_attempts = 5

if failed_attempts > 3:
    print("Account requires review")
else:
    print("Account is normal")


# Task 3: Use a loop

login_attempts = [1, 2, 3, 4, 5]

for attempt in login_attempts:
    print("Reviewing login attempt:", attempt)


# Task 4: Create a function

def check_login_status(attempts):
    if attempts > 3:
        return "Suspicious activity detected"
    else:
        return "No issues detected"

result = check_login_status(5)

print(result)
```

## Takeaways

- Learned the basics of Python programming for cybersecurity tasks.
- Practiced creating variables and working with different data types.
- Used conditional statements to make decisions based on security conditions.
- Used loops to automate repetitive tasks.
- Created functions to organize and reuse Python code.
- Learned how Python can help security analysts automate investigations and improve efficiency.
