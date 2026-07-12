# Create Loops

## Objective

Learn how to use Python loops to repeat actions, process multiple pieces of data, and automate repetitive cybersecurity tasks.

## Scenario

As a security analyst, loops can help automate tasks such as reviewing multiple login attempts, scanning lists of IP addresses, and analyzing security events. In this lab, Python `for` and `while` loops were used to repeat actions and process data efficiently.

## Tools Used

- Python
- Jupyter Notebook
- Loops
- for Loop
- while Loop
- Lists
- Range Function

## Python Code

```python
# Task 1: Use a for loop to review login attempts

login_attempts = [1, 2, 3, 4, 5]

for attempt in login_attempts:
    print("Reviewing login attempt:", attempt)


# Task 2: Use a for loop with range()

for number in range(1, 6):
    print("Security check number:", number)


# Task 3: Use a while loop

failed_attempts = 0

while failed_attempts < 5:
    failed_attempts += 1
    print("Failed login attempt:", failed_attempts)


# Task 4: Loop through suspicious IP addresses

suspicious_ips = [
    "192.168.1.10",
    "10.0.0.5",
    "172.16.0.8"
]

for ip in suspicious_ips:
    print("Reviewing suspicious IP:", ip)
```

## Takeaways

- Learned how to create and use loops in Python.
- Practiced using `for` loops to process lists of information.
- Used `while` loops to repeat actions until a condition is met.
- Learned how loops can automate repetitive cybersecurity tasks.
- Improved Python skills for analyzing large amounts of security data.
