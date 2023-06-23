# Multiple Inheritance in Python
Multiple inheritance is a powerful feature in object-oriented programming that allows a class to inherit attributes and methods from multiple parent classes. This can be useful in situations where a class needs to inherit functionality from multiple sources.


## Syntax
In Python, multiple inheritance is implemented by specifying multiple parent classes in the class definition, separated by commas.
```python
class ChildClass(ParentClass1, ParentClass2, ParentClass3):
    # class body
```

In this example, the `ChildClass` inherits attributes and methods from all three parent classes: `ParentClass1`, `ParentClass2`, and `ParentClass3`.

It's important to note that, in case of multiple inheritance, Python follows a `method resolution order (MRO)` to resolve conflicts between methods or attributes from different parent classes. The MRO determines the order in which parent classes are searched for attributes and methods. 

## Example
```python
class Animal:
    def __init__(self, name, species):
        self.name = name
        self.species = species
        
    def make_sound(self):
        print("Sound made by the animal")
        
class Mammal:
    def __init__(self, name, fur_color):
        self.name = name
        self.fur_color = fur_color
        
class Dog(Animal, Mammal):
    def __init__(self, name, breed, fur_color):
        Animal.__init__(self, name, species="Dog")
        Mammal.__init__(self, name, fur_color)
        self.breed = breed
        
    def make_sound(self):
        print("Bark!")
```
In this example, the `Dog` class inherits from both the `Animal` and `Mammal` classes, so it can use attributes and methods from both parent classes.
## [Next Lesson>>](https://replit.com/@codewithharry/80-Day-80-Multilevel-Inheritance)