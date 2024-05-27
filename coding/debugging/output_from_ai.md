The provided Python function `is_prime` has a few errors that need to be fixed:

1. The loop should only go up to the square root of the number, not to the number itself. This optimization reduces the number of iterations.
2. The loop should include the square root of the number as a potential factor.
3. An additional test case is included for 20 but it doesn't have a closing parenthesis.

Here is the corrected code:

```python
import math

def is_prime(num):
    if num <= 1:
        return False
    for i in range(2, int(math.sqrt(num)) + 1):
        if num % i == 0:
            return False
    return True
```

#### Test cases
- print(is_prime(1))  # Expected output: False
- print(is_prime(2))  # Expected output: True
- print(is_prime(4))  # Expected output: False
- print(is_prime(17))  # Expected output: True
- print(is_prime(20))  # Expected output: False

These changes ensure the function correctly identifies prime numbers and is more efficient.
