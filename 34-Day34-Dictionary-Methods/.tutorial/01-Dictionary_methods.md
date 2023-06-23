# Dictionary Methods
Dictionary uses several built-in methods for manipulation.They are listed below
## update() 
The update() method updates the value of the key provided to it if the item already exists in the dictionary, else it creates a new key-value pair.

#### Example:
```python
info = {'name':'Karan', 'age':19, 'eligible':True}
print(info)
info.update({'age':20})
info.update({'DOB':2001})
print(info)
```
#### Output:
```
{'name': 'Karan', 'age': 19, 'eligible': True}
{'name': 'Karan', 'age': 20, 'eligible': True, 'DOB': 2001}
 ```

 

## Removing items from dictionary:
There are a few methods that we can use to remove items from dictionary.

 

### clear():
The clear() method removes all the items from the list. 
#### Example:
```python
info = {'name':'Karan', 'age':19, 'eligible':True}
info.clear()
print(info)
```
#### Output:
```
{}
 ```

#### pop():
The pop() method removes the key-value pair whose key is passed as a parameter.
#### Example:
```python
info = {'name':'Karan', 'age':19, 'eligible':True}
info.pop('eligible')
print(info)
```
#### Output:
```
{'name': 'Karan', 'age': 19}
 ```

### popitem(): 
The popitem() method removes the last key-value pair from the dictionary.
#### Example:
```python
info = {'name':'Karan', 'age':19, 'eligible':True, 'DOB':2003}
info.popitem()
print(info)
```
#### Output:
```
{'name': 'Karan', 'age': 19, 'eligible': True}
 ```

### del:
we can also use the del keyword to remove a dictionary item. 

#### Example:
```python
info = {'name':'Karan', 'age':19, 'eligible':True, 'DOB':2003}
del info['age']
print(info)
```
#### Output:
```
{'name': 'Karan', 'eligible': True, 'DOB': 2003}
 ```

If key is not provided, then the del keyword will delete the dictionary entirely.

#### Example:
```python
info = {'name':'Karan', 'age':19, 'eligible':True, 'DOB':2003}
del info
print(info)
```
#### Output:
```
NameError: name 'info' is not defined
```
## [Next Lesson>>](https://replit.com/@codewithharry/35-Day-35-For-loop-with-else)