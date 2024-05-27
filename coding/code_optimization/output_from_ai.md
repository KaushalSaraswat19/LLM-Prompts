Here's the optimized version of the Fibonacci function using memoization:

```python
def fibonacci(n, memo={}):
    """
    Calculates the nth Fibonacci number using memoization.
    
    Parameters:
        n (int): The index of the Fibonacci number to compute.
        memo (dict): A dictionary to store computed Fibonacci numbers.
    
    Returns:
        int: The nth Fibonacci number.
    """
    if n in memo:
        return memo[n]
    if n <= 1:
        return n
    else:
        memo[n] = fibonacci(n - 1, memo) + fibonacci(n - 2, memo)
        return memo[n]

# Test cases
print(fibonacci(5))  # Expected output: 5
print(fibonacci(10)) # Expected output: 55
print(fibonacci(20)) # Expected output: 6765
```

Explanation:

- In the optimized version, we added an additional parameter `memo` to the function to store computed Fibonacci numbers.
- Inside the function, we first check if the result for the current `n` is already stored in the `memo`. If it is, we return the cached result.
- If `n` is less than or equal to 1, we return `n` directly.
- Otherwise, we recursively calculate `fibonacci(n - 1, memo)` and `fibonacci(n - 2, memo)` while storing the results in the `memo` dictionary.
- By memoizing previously computed Fibonacci numbers, we avoid redundant calculations and significantly improve the performance of the function, especially for larger values of `n`.