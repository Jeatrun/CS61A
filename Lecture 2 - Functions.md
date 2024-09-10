# Lecture 2 - Functions

##  1.call expression

```python
"""
call expressions are functions
  max     (   2    ,   3    )
--------   -------- --------
operator   operand  operand

Note: operands could also be call expressions
max(add(1, 2), mul(3, 4))
"""
from operator import add,mul
"""
>>>add(2,3)
5
"""

```

## 2.Names, Assignment, and User-defined Functions

```python
"""
Names are variables 
We use '=' to assign data to them
"""
radius = 10
"""
>>> radius
10
"""
```

```python
"""
Use 'def' to create user-defined functions
>>def <name>(<parameters>):
	return <return exoression>
"""
def square(x):
    return mul(x,x)
"""
>>> square(4)
16
"""

```

## 3.Environment & Frames



```python
"""
- Environment is *a sequence of Frames* 
- When we use a name,we would first go to find in the local frame, then go to the global frame

"""
def square(square):
    return mul(square,square)

square(-2)
"""
|square          ->local frame
|  square |-2    ->local variables (parameter)   

- in this case, square has been bound to a user-defined function and the parameter

- when execute this function, we create a new frame call "square"

-then, we go to find parameter "square" in the frame "square" and bind the value "-2" to it
"""
```

 



