# Single Inheritance in Python
Single inheritance is a type of inheritance where a class inherits properties and behaviors from a single parent class. This is the simplest and most common form of inheritance.

## Syntax
The syntax for single inheritance in Python is straightforward and easy to understand. To create a new class that inherits from a parent class, simply specify the parent class in the class definition, inside the parentheses, like this:

```python
class ChildClass(ParentClass):
    # class body

```

## Example
Let's consider a simple example of single inheritance in Python. Consider a class named "Animal" that contains the attributes and behaviors that are common to all animals.
```python
class Animal:
    def __init__(self, name, species):
        self.name = name
        self.species = species
        
    def make_sound(self):
        print("Sound made by the animal")
```

If we want to create a new class for a specific type of animal, such as a dog, we can create a new class named "Dog" that inherits from the Animal class.

```python
class Dog(Animal):
    def __init__(self, name, breed):
        Animal.__init__(self, name, species="Dog")
        self.breed = breed
        
    def make_sound(self):
        print("Bark!")
```
The Dog class inherits all the attributes and behaviors of the Animal class, including the `__init__` method and the `make_sound` method. Additionally, the Dog class has its own `__init__` method that adds a new attribute for the breed of the dog, and it also overrides the `make_sound` method to specify the sound that a dog makes.


Single inheritance is a powerful tool in Python that allows you to create new classes based on existing classes. It allows you to reuse code, extend it to fit your needs, and make it easier to manage complex systems. Understanding single inheritance is an important step in becoming proficient in object-oriented programming in Python.
## [Next Lesson>>](https://replit.com/@codewithharry/79-Day-79-Multiple-Inheritance)