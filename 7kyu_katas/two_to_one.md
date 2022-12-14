# CodeWars Python Solutions

---

## Two to One

Take 2 strings `s1` and `s2` including only letters from `a` to `z`. Return a new sorted string, the longest possible, containing distinct letters,

- each taken only once - coming from s1 or s2.


**Examples**

```
a = "xyaabbbccccdefww"
b = "xxxxyyyyabklmopq"

longest(a, b) -> "abcdefklmopqwxy"

a = "abcdefghijklmnopqrstuvwxyz"

longest(a, a) -> "abcdefghijklmnopqrstuvwxyz"
```

---

### Given Code


```python
def longest(s1, s2):
    pass
```

---

### Solution 1


```python
def longest(s1, s2):
    return "".join(sorted([c for c in set(s1 + s2)]))
```

### Solution 2


```python
def longest(a1, a2):
    return "".join(sorted(set(a1 + a2)))
```

---


[See on CodeWars.com](https://www.codewars.com/kata/5656b6906de340bd1b0000ac/)
