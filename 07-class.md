# Introduction to Enums in Python
Enums, short for Enumerations, are a feature in Python that lets you define a set of named values. This can be handy when you have a variable that should only hold a few specific values, like days of the week or types of fruits. The enum module, available from Python 3.4, provides the Enum class for creating these sets.  
### example:
    from enum import Enum

    class Fruit(Enum):
    APPLE = 1
    BANANA = 2
    CHERRY = 3

#### With this, you can do things like:  

    print(Fruit.APPLE)
    print(Fruit.APPLE.name)
    print(Fruit.APPLE.value)

#### This will print:
    Fruit.APPLE
    APPLE
    1

### Enums Advantage:

Using Enums makes your code:
 - cleaner  
 - helps prevent mistakes by limiting the values a variable can take.


 # The SOLID principles 
 The SOLID principles, introduced by Robert C. Martin (Uncle Bob), are a set of design guidelines aimed at making software designs more understandable, flexible, and maintainable. Here’s a brief explanation of each principle with Python examples:

1. single Responsibility Principle (SRP)

    - A class should have only one reason to change, meaning it should have only one job or responsibility.

2. open/Closed Principle (OCP)
    - Software entities should be open for extension but closed for modification.
  
3. Liskov Substitution Principle (LSP)
    - Subtypes must be substitutable for their base types without altering the correctness of the program.

4. Interface Segregation Principle (ISP)
     - clients should not be forced to depend on interfaces they do not use

5. Dependency Inversion Principle (DIP)

    -high-level modules should not depend on low-level modules. Both should depend on abstractions.

