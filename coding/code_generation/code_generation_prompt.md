# Code Generation Prompt

## Description
Automatically generate code snippets in various programming languages based on user-specified requirements. This prompt is invaluable for developers seeking to streamline their workflow by automating the generation of code tailored to different programming languages, frameworks, or specific project needs.

## Prompt
Write a Python function named `bubble_sort` that takes a list of integers as input and sorts it in ascending order using the Bubble Sort algorithm. You can assume the input list will contain at least one integer.

The Bubble Sort algorithm works by repeatedly stepping through the list, comparing adjacent elements, and swapping them if they are in the wrong order. The pass through the list is repeated until the list is sorted.

Your function should modify the input list in place and return nothing.

#### Example Usage:
```python
# Example usage of the generated function
my_list = [3, 1, 5, 2, 4]
bubble_sort(my_list)
print(my_list)  # Expected output: [1, 2, 3, 4, 5]
```

#### Constraints (optional for more accuracy)
- the implementation should use the Bubble Sort algorithm.
- Do not use built-in sorting functions or libraries.
- The input list will contain only integers.