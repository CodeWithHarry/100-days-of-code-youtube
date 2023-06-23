# Hierarchical Inheritance

Hierarchical Inheritance is a type of inheritance in Object-Oriented Programming where multiple subclasses inherit from a single base class. In other words, a single base class acts as a parent class for multiple subclasses. This is a way of establishing relationships between classes in a hierarchical manner.

Here's an example to illustrate the concept of hierarchical inheritance in Python:
```python
class Animal:
    def __init__(self, name):
        self.name = name

    def show_details(self):
        print("Name:", self.name)

class Dog(Animal):
    def __init__(self, name, breed):
        Animal.__init__(self, name)
        self.breed = breed

    def show_details(self):
        Animal.show_details(self)
        print("Species: Dog")
        print("Breed:", self.breed)

class Cat(Animal):
    def __init__(self, name, color):
        Animal.__init__(self, name)
        self.color = color

    def show_details(self):
        Animal.show_details(self)
        print("Species: Cat")
        print("Color:", self.color)
```
In the above code, the `Animal` class acts as the base class for two subclasses, `Dog` and `Cat`. The `Dog` class and the `Cat` class inherit the attributes and methods of the `Animal` class. However, they can also add their own unique attributes and methods.

Here's an example of creating objects of the `Dog` and `Cat` classes and accessing their attributes and methods:

```python
dog = Dog("Max", "Golden Retriever")
dog.show_details()
cat = Cat("Luna", "Black")
cat.show_details()
```
### Output:
```
Name: Max
Species: Dog
Breed: Golden Retriever
Name: Luna
Species: Cat
Color: Black
```
As we can see from the outputs, the `Dog` and `Cat` classes have inherited the attributes and methods of the `Animal` class, and have also added their own unique attributes and methods.

In conclusion, hierarchical inheritance is a way of establishing relationships between classes in a hierarchical manner. It allows multiple subclasses to inherit from a single base class, which helps in code reuse and organization of code in a more structured manner.
## [Next Lesson>>](https://replit.com/@codewithharry/82-Day-82-Exercise-8-Solution)



