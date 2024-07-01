# Keywords

**Encapsulation**: This is a fundamental principle of OOP that involves bundling the data (variables) and methods (functions) that operate on the data into a single unit, typically a class. Encapsulation restricts direct access to some of an object's components, which is a means of preventing unintended interference and misuse of the methods and data.

**Inheritance**: This is a mechanism where a new class is derived from an existing class. The new class, known as the subclass (or derived class), inherits attributes and methods of the existing class, referred to as the superclass (or base class). This promotes code reuse and establishes a relationship between classes.

**Polymorphism**: This allows objects of different classes to be treated as objects of a common super class. It is most often used in the context of inheritance. Polymorphism means "many shapes" and it allows methods to do different things based on the object it is acting upon, even if they share the same name.

**Abstraction**: This is the concept of hiding the complex implementation details and showing only the necessary features of the object. It helps in reducing programming complexity and effort.

**Class**: A class is a blueprint for creating objects (a particular data structure), providing initial values for state (member variables or fields), and implementations of behavior (member functions or methods).

**Method**: A method is a function defined within a class. It describes the behaviors of the objects created from the class.

# Symbols

**+**: In UML (Unified Modeling Language) class diagrams, a plus sign (+) indicates that a member (field or method) is public. This means it is accessible from any other class.

**-**: A minus sign (-) indicates that a member is private. This means it is only accessible within the class it is defined in.

**|**: Vertical bars are used to frame the structure of the class and the entire diagram. They represent the borders of the diagram's components.

**+--------------+**: Horizontal bars are used to separate different sections of the diagram, such as the name of the class from its attributes and methods.

**Inherits**: This keyword signifies the inheritance relationship between two classes, indicating that one class derives from another.

**^**: The caret symbol represents the direction of inheritance in the diagrams, pointing from the derived class to the base class.


# Four Pillars of OOP in Java

## Encapsulation and Inheritance
```plaintext
+---------------------+         +---------------------+
|     Encapsulation   |         |     Inheritance     |   
+---------------------+         +---------------------+
| +----------------+  |         |  +--------------+   |
| | Person Class   |  |         |  | Animal Class |   |
| +----------------+  |         |  +--------------+   |
| | - name: String |  |         |  | + eat()      |   |
| | - age: int     |  |         |  +--------------+   |
| | + getName()    |  |         |         |            |
| | + setName()    |  |         |         | Inherits   |
| | + getAge()     |  |         |         v            |
| | + setAge()     |  |         |  +--------------+   |
| +----------------+  |         |  | Dog Class    |   |
+---------------------+         |  +--------------+   |
                                |  | + bark()     |   |
                                |  +--------------+   |
                                +---------------------+


+---------------------+         +---------------------+
|     Polymorphism    |         |     Abstraction     |
+---------------------+         +---------------------+
| +----------------+  |         | +----------------+  |
| | Animal Class   |  |         | | Vehicle Class  |  |
| +----------------+  |         | +----------------+  |
| | + makeSound()  |  |         | | + start() (abs)|  |
| +----------------+  |         | | + stop()       |  |
|         ^            |         | +----------------+  |
|         |            |         |         ^            |
|         | Polymorphism|         |         | Inherits   |
|         |            |         |         v            |
| +----------------+  |         | +----------------+  |
| | Cat Class      |  |         | | Car Class      |  |
| +----------------+  |         | +----------------+  |
| | + makeSound()  |  |         | | + start()      |  |
| +----------------+  |         | +----------------+  |
+---------------------+         +---------------------+


