# Lecture 3 - Control

## 3.1 Print & None

```python
"""
- Print is a "unpure function",which has a side effect: print the values
- When execute the print,it will print the value first,then return the return value "None"
"""
print(print(1), print(2))
"""
1
2
None None
"""

```

 ## 3.2 Miscellaneous Python Functions

### 3.2.1 true division and integer(floor) division

```python
td=2024/10
fd=2024//10
from operator import truediv,floordiv
tdf=truediv(2024,10)
fdf=floordiv(2024,10)
"""
>>> print(td,fd,tdf,fdf)
202.4
202
202.4
202
"""
```

### 3.2.2 Multiple returns  & default values

```python
"""
- in python, we could return multiple values
return <value1>, <value2> .....
- we could aslo assign default values to parameters like 'd=10'
"""
def divide_exact(n,d=10):
    """
    >>>quotient, remainder = divide_exact(2024,10)
    >>>quotient
    202
    >>>remainder
    4
    """
    return n // d, n % d
quotient, remainder = divide_exact(2024,10)

```

## 2.2.3  interactive & doc test

use `python3 -i [file]`  to run a program interactively

use `python3 -m doctest [file]` to run a doc test

