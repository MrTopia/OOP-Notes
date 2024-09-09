# OOP-Notes
1.Compare procedural programming with object oriented programming for what type of Application is the procedural programming is suitable and for what type OOP is suitable? Justify Your answer.

Ans - Procedural programming and object-oriented programming (OOP) are two distinct paradigms used in software development, each with its own strengths and weaknesses. The choice between the two depends largely on the nature of the application being developed.

Procedural Programming

 * Focus: Breaks down problems into a series of steps or procedures that are executed sequentially.

 * Data: Data is treated as separate entities from the procedures.

 * Suitability: Applications where the flow of control is linear and the data is relatively simple. Examples include:

   * System utilities (e.g., file managers, text editors)

   * Numerical computations (e.g., scientific simulations, data analysis)

   * Command-line applications

Object-Oriented Programming

 * Focus: Models real-world entities as objects that interact with each other.

 * Data and Procedures: Data and the procedures that operate on it are encapsulated within objects.

 * Suitability: Applications that involve complex relationships between entities and require code reusability. Examples include:

   * Graphical user interfaces (GUIs)

   * Games

   * Large-scale enterprise systems

   * Web applications

2. Describe how data are shared by functions in procedure-oriented programs?

Ans – In procedure-oriented programs, data is typically shared between functions using global variables or parameter passing.

Global Variables:

 * Global variables are declared outside of any function and can be accessed from anywhere within the program.

 * This means that functions can modify the values of global variables, which can lead to unintended side effects if not used carefully.

Parameter Passing:

 * Functions can also share data by passing arguments to each other.

 * There are two main ways to pass arguments: call by value and call by reference.

 * Call by value: A copy of the argument’s value is passed to the function. Any changes made to the argument within the function do not affect the original value.

 * Call by reference: A reference to the argument’s memory location is passed to the function. This means that any changes made to the argument within the function will affect the original value.

3. Distinguish between the following terms:

(a)	Object and classes

(b)	Data abstraction and data encapsulation

(c)	 Inheritance and polymorphism

(d)	Dynamic binding and message passing

Ans- Object-Oriented Programming Concepts

(a) Object and Classes

 * Object: An object is a real-world entity with a unique identity, attributes, and behaviors. It represents an instance of a class. For example, a “car” is an object with attributes like color, make, model, and behaviors like start, stop, accelerate, and brake.

 * Class: A class is a blueprint or template that defines the common properties (attributes) and behaviors (methods) of a group of objects. It serves as a logical grouping of objects with similar characteristics. For example, the “Car” class would define the common attributes and behaviors for all cars.

(b) Data Abstraction and Data Encapsulation

 * Data Abstraction: Data abstraction focuses on the essential characteristics of an object, hiding the unnecessary details. It allows you to work with objects at a higher level of abstraction, making the code easier to understand and maintain. For example, when using a car object, you only need to know how to start, stop, and drive it, without worrying about the internal mechanisms.

 * Data Encapsulation: Data encapsulation is the mechanism of binding data (attributes) and methods (behaviors) together within a class and controlling access to them. It ensures that the internal state of an object is protected from unauthorized access, making the code more secure and reliable. Encapsulation is achieved through access modifiers like public, private, and protected.

© Inheritance and Polymorphism

 * Inheritance: Inheritance is a mechanism where a class can acquire the properties and behaviors of another class. It promotes code reusability and creates a hierarchical relationship between classes. The derived class (child class) inherits the members of the base class (parent class). For example, a “Truck” class can inherit from the “Vehicle” class, acquiring properties like color, make, and model, as well as behaviors like start, stop, and drive.

 * Polymorphism: Polymorphism means the ability of objects of different classes to respond to the same message in different ways. It allows you to write more flexible and adaptable code. There are two types of polymorphism:

   * Compile-time polymorphism: Achieved through method overloading (defining methods with the same name but different parameters within the same class).

   * Runtime polymorphism: Achieved through method overriding (defining methods with the same name and signature in both the base and derived classes).

(d) Dynamic Binding and Message Passing

 * Dynamic Binding: Dynamic binding, also known as late binding, is the process of determining the method to be executed at runtime based on the actual object type. This allows for flexibility and polymorphism. In dynamic binding, the decision about which method to call is made at runtime based on the object’s type.

 * Message Passing: Message passing is the mechanism of sending a message to an object, requesting it to perform a specific action. The object receives the message, interprets it, and invokes the appropriate method to carry out the requested action. Message passing is the fundamental way objects interact with each other in object-oriented programming.





4. What do mean by abstract class and container class? Describe their use with the help of c++ Program?

Ans- 

Abstract Classes

 * Definition: An abstract class is a class that cannot be directly instantiated. It serves as a blueprint for other classes, providing a common interface and defining the structure of derived classes.

 * Key Characteristics:

   * Contains at least one pure virtual function.

   * Cannot be used to create objects directly.

   * Must be inherited by concrete classes to be useful.

 * Purpose:

   * Defines a common interface for related classes.

   * Enforces a consistent structure and behavior among derived classes.

   * Promotes code reusability and maintainability.

Container Classes

 * Definition: Container classes are specialized data structures that store and manage collections of elements. They provide efficient operations for inserting, removing, searching, and iterating over elements.

 * Common Types:

   * Vector: Dynamically resizable array.

   * List: Doubly linked list.

   * Deque: Double-ended queue.

   * Set: Unordered collection of unique elements.

   * Map: Associates keys with values.

   * Multiset: Unordered collection of elements, allowing duplicates.

   * Multimap: Associates keys with multiple values.

 * Benefits:

   * Simplify complex data management tasks.

   * Provide efficient algorithms for various operations.

   * Enhance code readability and maintainability.

5. How does a main () function in c++ differ from main () in c?

Ans – 

C:

 * Prototype: int main(void)

 * Return Type: int (typically indicating success or failure)

 * Parameters: None

 * Purpose: The entry point of the program. Execution begins here.

C++:

 * Prototype: int main() or int main(int argc, char* argv[])

 * Return Type: int (same as C)

 * Parameters:

   * int argc: Number of command-line arguments passed to the program.

   * char* argv[]: Array of strings containing the command-line arguments.

 * Purpose: Similar to C, the entry point of the program. However, it can also be overloaded with different parameter lists.

Key Differences:

 * Parameters: C++ allows the main() function to accept command-line arguments, while C requires a fixed prototype without parameters.

 * Overloading: C++ supports function overloading, so you can define multiple main() functions with different parameter lists. This is not possible in C.

 * Namespace: In C++, main() is typically defined within the std namespace. In C, there is no concept of namespaces.



6. When is an object created and what is its lifetime?

Ans – Object Creation and Lifetime

In programming, an object is an instance of a class. Its creation and lifetime are fundamental concepts in object-oriented programming.

When is an object created?

An object is typically created when:

•	A class instance is explicitly declared:

   MyClass object = new MyClass();



 * A class instance is created implicitly:

   * In certain languages, objects might be created automatically in specific contexts, such as when a function returns an object or when an object is used as a parameter.

 * A class instance is created using a factory method:

   * A factory method is a static method that returns an object of a specific class.

Object Lifetime

The lifetime of an object refers to the period between its creation and its destruction. The object’s lifetime is determined by the garbage collector or explicit deallocation mechanisms in the programming language.

 * Garbage Collection:

   * Many modern programming languages (like Java, Python, and C#) employ automatic garbage collection. The garbage collector periodically scans memory for objects that are no longer referenced by any active code. When it finds such objects, it reclaims the memory they occupy.

 * Explicit Deallocation:

   * In languages like C and C++, manual memory management is required. Programmers must explicitly allocate memory for objects using malloc or new and deallocate it using free or delete when the object is no longer needed. Failure to deallocate memory can lead to memory leaks.

Factors Affecting Object Lifetime:

 * Scope: The scope of a variable or object determines its visibility and lifetime within a program. Objects declared within a block or function have a limited lifetime, often tied to the execution of that block or function.

 * References: As long as there are references to an object, it will not be garbage collected. If all references to an object are lost, it becomes eligible for collection.

 * Explicit Destruction: In languages with manual memory management, the programmer must explicitly deallocate objects to prevent memory leaks.

Understanding object creation and lifetime is crucial for writing efficient and memory-safe code. By managing object lifetimes effectively, you can avoid memory-related issues and optimize your program’s performance.



9. Explain the purpose of new and delete operator by using C++ program.

Ans- The new and delete operators in C++ are used for dynamic memory allocation and deallocation, respectively.

New operator:

 * Allocates memory on the heap for a specified data type.

 * Returns a pointer to the allocated memory.

 * Can be used to create objects of classes.

Delete operator:

 * Deallocates memory previously allocated using new.

 * Takes a pointer to the memory to be deallocated as an argument.

 * Prevents memory leaks.

10. What do you mean by dynamic binding? How it is useful in OOP?

Ans - Dynamic binding is a mechanism in object-oriented programming (OOP) where the method to be called is determined at runtime based on the object's actual type. This allows for greater flexibility and polymorphism, as the same code can work with objects of different classes that share a common interface.





It's useful in OOP because:

 * Polymorphism: It enables different objects to be treated as if they were of the same type, allowing for more generic code.

 * Flexibility: It makes it easier to add new classes or modify existing ones without affecting existing code.

 * Code reusability: It promotes code reuse by allowing you to write code that works with objects of different classes.

