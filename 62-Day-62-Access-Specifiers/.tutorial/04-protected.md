# Protected Access Modifier  
In object-oriented programming (OOP), the term "protected" is used to describe a member (i.e., a method or attribute) of a class that is intended to be accessed only by the class itself and its subclasses. In Python, the convention for indicating that a member is protected is to prefix its name with a single underscore (_). For example, if a class has a method called _my_method, it is indicating that the method should only be accessed by the class itself and its subclasses.

It's important to note that the single underscore is just a naming convention, and does not actually provide any protection or restrict access to the member.
The syntax we follow to make any variable protected is to write variable name followed by a single underscore (_) ie. _varName.
## Example:
```python
class Student:
    def __init__(self):
        self._name = "Harry"

    def _funName(self):      # protected method
        return "CodeWithHarry"

class Subject(Student):       #inherited class
    pass

obj = Student()
obj1 = Subject()

# calling by object of Student class
print(obj._name)      
print(obj._funName())     
# calling by object of Subject class
print(obj1._name)    
print(obj1._funName()) 
```
## Output:
```
Harry
CodeWithHarry

Harry
CodeWithHarry
```
## [Next Lesson>>](https://replit.com/@codewithharry/63-Day-63-Exercise-5-Solution)