# Docstrings in python
Python docstrings are the string literals that appear right after the definition of a function, method, class, or module. 
## Example
```python
def square(n):
    '''Takes in a number n, returns the square of n'''
    print(n**2)
square(5)

```
Here, 

'''Takes in a number n, returns the square of n''' 
is a docstring which will not appear in output

## Output:
```
25
```
Here is another example:
```python
def add(num1, num2):
    """
    Add up two integer numbers.

    This function simply wraps the ``+`` operator, and does not
    do anything interesting, except for illustrating what
    the docstring of a very simple function looks like.

    Parameters
    ----------
    num1 : int
        First number to add.
    num2 : int
        Second number to add.

    Returns
    -------
    int
        The sum of ``num1`` and ``num2``.

    See Also
    --------
    subtract : Subtract one integer from another.

    Examples
    --------
    >>> add(2, 2)
    4
    >>> add(25, 0)
    25
    >>> add(10, -10)
    0
    """
    return num1 + num2
```
## Python Comments vs Docstrings
### Python Comments

Comments are descriptions that help programmers better understand the intent and functionality of the program. They are completely ignored by the Python interpreter.
### Python docstrings

As mentioned above, Python docstrings are strings used right after the definition of a function, method, class, or module (like in Example 1). They are used to document our code.

We can access these docstrings using the __doc__ attribute.
## Python __doc__ attribute
Whenever string literals are present just after the definition of a function, module, class or method, they are associated with the object as their __doc__ attribute. We can later use this attribute to retrieve this docstring.

## Example
```python
def square(n):
    '''Takes in a number n, returns the square of n'''
    return n**2

print(square.__doc__)
```
## Output:
Takes in a number n, returns the square of n