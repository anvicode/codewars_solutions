# How many lightsabers do you own?

## Task

Inspired by the development team at Vooza, write the function that accepts the name of a programmer, and returns the number of lightsabers owned by that person.
The only person who owns lightsabers is Zach, by the way. He owns 18, which is an awesome number of lightsabers. Anyone else owns 0.

Note: your function should have a default parameter.

**Examples:**

(Input --> Output):

```python
"anyone else" --> 0
"Zach" --> 18
```

## Given Code

```python
def how_many_light_sabers_do_you_own(name):
    return
```

## Solution

```python
def how_many_light_sabers_do_you_own(name=None):
    return 18 if name == "Zach" else 0
```

[See on Codewars](https://www.codewars.com/kata/51f9d93b4095e0a7200001b8/)
