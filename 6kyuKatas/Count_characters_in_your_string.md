# Count characters in your string

## Task

The main idea is to count all the occurring characters in a string. If you have a string like aba, then the result should be {'a': 2, 'b': 1}.

What if the string is empty? Then the result should be empty object literal, {}.

## Given Code

```python
def count(s):
    pass
```

## Solution

```python
def count(s):
    if len(s) == 0:
        return {}
    ht = {}
    for i in s:
        if i not in ht:
            ht[i] = 1
        else:
            ht[i] += 1
    return ht
```

[See on Codewars](https://www.codewars.com/kata/52efefcbcdf57161d4000091/)
