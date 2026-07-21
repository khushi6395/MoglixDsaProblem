# Longest Valid Parentheses

## Problem

Given a string containing only `'('` and `')'`, return the length of the longest valid parentheses substring.
Example

1.Input->
s = "(()"

Output
```
2
```

2. Input
```
s = ")()(()))"
```

Output
```
4
```

Input->
```
s = ""
```

Output->
```
0
```

## Approach

- Use a **Stack** to store the indices of `'('`.
- Push `-1` at the beginning to act as the starting index.
- If the current character is `'('`, push its index.
- If it is `')'`, pop the stack.
  - If the stack becomes empty, push the current index.
  - Otherwise, calculate the current valid substring length and update the maximum length.

## Time Complexity

- O(n)

## Space Complexity
O(n)




## Author

Khushi Sharma
