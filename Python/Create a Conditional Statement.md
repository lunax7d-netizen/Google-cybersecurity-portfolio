# Create a Conditional Statement

## Objective

Learn how to use Python conditional statements to make decisions based on specific conditions and automate security-related responses.

## Scenario

As a security analyst, conditional statements can be used to evaluate data and determine whether an action should be taken. In this lab, Python `if`, `elif`, and `else` statements were used to analyze security information and respond based on different conditions.

## Tools Used

- Python
- Jupyter Notebook
- Conditional Statements
- if
- elif
- else
- Comparison Operators

## Python Code

```python
# Check login attempts and determine if activity is suspicious

failed_attempts = 5

if failed_attempts > 5:
    print("Account requires immediate investigation")
elif failed_attempts >= 3:
    print("Review account activity")
else:
    print("No suspicious activity detected")


# Check if an account is locked

account_locked = True

if account_locked:
    print("Account is locked")
else:
    print("Account is active")
```

## Takeaways

- Learned how to create conditional statements in Python.
- Practiced using `if`, `elif`, and `else` statements to control program decisions.
- Learned how comparison operators can evaluate security-related data.
- Used conditions to automate responses based on different scenarios.
- Improved Python skills for analyzing and responding to cybersecurity events.
