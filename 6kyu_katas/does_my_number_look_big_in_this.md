# CodeWars Python Solutions

---

## Does my number look big in this?

**Definition**

A [Narcissistic Number](https://en.wikipedia.org/wiki/Narcissistic_number) is a number which is the sum of its own digits, each raised to the power of the number of digits in a given base. In this Kata, we will restrict ourselves to decimal (base 10).

For example, take 153 (3 digits):

```
1^3 + 5^3 + 3^3 = 1 + 125 + 27 = 153
```

and 1634 (4 digits):

```
1^4 + 6^4 + 3^4 + 4^4 = 1 + 1296 + 81 + 256 = 1634
```

**The Challenge:**

Your code must return true or false depending upon whether the given number is a Narcissistic number in base 10.

Error checking for text strings or other invalid inputs is not required, only valid integers will be passed into the function.

---

### Given Code

```python
def narcissistic( value ):
    pass
```

---

### Solution 1

```python
def narcissistic( value ):
    return value == sum([int(n) ** len(str(value)) for n in str(value)])
```

### Solution 2

```python
def narcissistic( value ):
    return True if value == sum([int(num)**len(str(value)) for num in str(value)]) else False
```

---

[See on CodeWars.com](https://www.codewars.com/kata/5287e858c6b5a9678200083c)
