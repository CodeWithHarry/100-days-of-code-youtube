# Tuple methods
As tuple is immutable type of collection of elements it have limited built in methods.They are explained below
## count() Method
The count() method of Tuple returns the number of times the given element appears in the tuple.

### Syntax:
```python
tuple.count(element)
```
### Example
```python
Tuple1 = (0, 1, 2, 3, 2, 3, 1, 3, 2)
res = Tuple1.count(3)
print('Count of 3 in Tuple1 is:', res)
```
### Output
3
# index() method
The Index() method returns the first occurrence of the given element from the tuple.

### Syntax:
```python
tuple.index(element, start, end)
```
Note: This method raises a ValueError if the element is not found in the tuple.

### Example
```python
Tuple = (0, 1, 2, 3, 2, 3, 1, 3, 2)
res = Tuple.index(3)
print('First occurrence of 3 is', res)
```
#### Output
3
## [Next Lesson>>](https://replit.com/@codewithharry/26-Day-26-Exercise-2-Solution)