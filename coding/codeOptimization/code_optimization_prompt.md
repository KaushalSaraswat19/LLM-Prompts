# Code Optimization Prompt

## Description
Optimize the given code snippet to improve its performance and efficiency across various factors, including algorithmic complexity, memory usage, and execution speed. This challenge is designed to help developers enhance their optimization skills and produce high-performance code in any programming language.

## Prompt
You are provided with a Python function that computes the nth Fibonacci number using a recursive approach. Your task is to optimize the code to reduce its time complexity, memory usage, and execution time while maintaining the same functionality.

```python
def fibonacci(n):
    """
    Calculates the nth Fibonacci number using recursion.
    
    Parameters:
        n (int): The index of the Fibonacci number to compute.
    
    Returns:
        int: The nth Fibonacci number.
    """
    if n <= 1:
        return n
    else:
        return fibonacci(n - 1) + fibonacci(n - 2)
```

#### Test cases (optional for more accuracy)
- print(fibonacci(5)) # Expected output: 5
- print(fibonacci(10)) # Expected output: 55
- print(fibonacci(20)) # Expected output: 6765

#### Constraints (if needed)
- The optimized code should produce the same output as the original function.
- Focus on improving time complexity, memory usage, and overall execution speed.
- Consider algorithmic optimizations, loop optimizations, memory management, and any other relevant factors.
- The function should handle non-negative integer inputs.