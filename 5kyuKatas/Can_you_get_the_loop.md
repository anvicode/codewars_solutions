# Can you get the loop ?

## Task

You are given a node that is the beginning of a linked list. This list contains a dangling piece and a loop. Your objective is to determine the length of the loop.

For example in the following picture the size of the dangling piece is 3 and the loop size is 12:

![](https://i.imgur.com/anTn5lG.png)

```python
# Use the `next' attribute to get the following node
node.next
```

Notes:

- do NOT mutate the nodes!

- in some cases there may be only a loop, with no dangling piece

> Thanks to shadchnev, I broke all of the methods from the Hash class.

> Don't miss dmitry's article in the discussion after you pass the Kata !!

## Given Code

```python
def loop_size(node):
    pass
```

## Solution

```python
def loop_size(node):
    s, f = node.next, node.next.next
    while s != f:
        s = s.next
        f = f.next.next
    ls = 1
    f = f.next
    while s != f:
        f = f.next
        ls += 1
    return ls
```

[See on Codewars](https://www.codewars.com/kata/52a89c2ea8ddc5547a000863/)
