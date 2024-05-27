# Debugging Prompt

## Description
Identify and fix errors in the given code. This prompt is useful for developers to practice finding and resolving bugs in their code.

## Prompt
You are given a Python function that is supposed to check if a number is prime. However, there are some errors in the code. Identify and fix the errors.

```python
def is_prime(num):
    if num <= 1:
        return False
    for i in range(2, num):
        if num % i == 0:
            return False
    return True
```

#### Test cases (optional)
- print(is_prime(1))  # Expected output: False
- print(is_prime(2))  # Expected output: True
- print(is_prime(4))  # Expected output: False
- print(is_prime(17))  # Expected output: True
- print(is_prime(20))  # Expected output: False
