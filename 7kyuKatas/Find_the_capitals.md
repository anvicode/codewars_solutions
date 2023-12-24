# Find the capitals

## Task

### Instructions

Write a function that takes a single string (word) as argument. The function must return an ordered list containing the indexes of all capital letters in the string.

### Example (Input --> Output)

`"CodEWaRs" --> [0,3,4,6]`

## Given Code

```python
def capitals(word):
    ...
```

## Solution

```python
def capitals(word):
    res = []
    for i, v in enumerate(word):
        if v == v.capitalize():
            res.append(i)
    return res
```

[See on Codewars](https://www.codewars.com/kata/539ee3b6757843632d00026b/)
