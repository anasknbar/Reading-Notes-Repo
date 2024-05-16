# Object-Oriented Programming-OOP

- in programming, we hve a lot of coding paradigm that we can use to acheive our goal. 
object-oriented programming is a programming paradigm that provides a means of writing programs so that properties and behaviors are bundled/encapsulated into individual objects.

- object-oriented programming is an approach for modeling real-world entities, like animals. 

- what are  class and instance mean in OOP?
A class is a blueprint for how to define something. It doesn’t actually contain any data. For example, If you make class for Dog doesn’t contain name or age or ...etc of any specific dog.The Dog class specifies that a name and an age and other attributes are necessary for defining a dog.

- While the class is the blueprint, an instance is an object that’s built from a class and contains real data. An instance of the class is not a blueprint anymore. It’s an actual attriputes of the real-world entity.

# How to define a class in python? 

    class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def greet(self):
        return f"Hello, my name is {self.name} and I'm {self.age} years old."
- The _ _init_ _ method (magic/dunder method) is a special method used for initializing objects. It is called automatically when a new instance of the class is created.

# How to creating instance/object out of the class?

    person1 = Person("Ali", 30)
    person2 = Person("Mohammad", 25)

# How to access attributes and calling methods??

You can access attributes and call methods using the dot notation (object.attribute) or (object.method()).

    print(person1.name)
    print(person2.name)

 
# Inheritance

- Inheritance allows a class (subclass) to inherit attributes and methods from another class (superclass).
- super() function is used to call the superclass's methods.

# dunder methods

## _ _str_ _ and _ _repr_ _

The __str__ method is called when the str() function is used or when an object is converted to a string implicitly. It should return a human-readable string representation of the object.

The __repr__ method is called by the repr() function or when an object is displayed in the interpreter. It should return an unambiguous string representation of the object that could be used to recreate the object.

## _ _len_ _

The __len__ method is called when the len() function is used on an object. It should return the length of the object.

## _ _getitem_ _ 

return the indexed item usnig the object[index] .

 

