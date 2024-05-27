Sure, here's a detailed solution for the Bubble Sort algorithm implemented in Python:
```python
def bubble_sort(arr):
    n = len(arr)
    # Traverse through all array elements
    for i in range(n):
        # Last i elements are already in place, so we don't need to check them again
        for j in range(0, n-i-1):
            # Traverse the array from 0 to n-i-1
            # Swap if the element found is greater than the next element
            if arr[j] > arr[j+1]:
                arr[j], arr[j+1] = arr[j+1], arr[j]

# Example usage
my_list = [3, 1, 5, 2, 4]
bubble_sort(my_list)
print(my_list)  # Output: [1, 2, 3, 4, 5]
```

### Explanation:

- The function `bubble_sort` takes a list `arr` as input.
- `n = len(arr)` gets the length of the input list.
- The outer loop runs `n` times, ensuring that after each iteration, the largest element gets placed at the end of the list (similar to a bubble rising to the surface).
- The inner loop compares adjacent elements and swaps them if they are in the wrong order. This process "bubbles" the largest element to the end.
- The function modifies the input list `arr` in place, sorting it in ascending order.