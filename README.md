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


12.What do you mean by operator overloading and method overloading? Write a distance class which contains data members of distance in meters, centimeters and millimeters. The class must Have overloaded operators for addition + and subtraction- respectively.

14.Explain the following terms in the context of object oriented programming. Also explain how These concepts are implemented in C++ by giving an example program for each.
(a)Benefits of Data Abstraction
(b)Encapsulation
(c) Virtual base class and when do we make it.
(d )Polymorphism and its types.

Ans- ### (a) Benefits of Data Abstraction
**Data abstraction** is the process of hiding the complex implementation details and showing only the necessary features of an object. It simplifies code and improves security by exposing only relevant data and methods.

**Benefits**:
1. Simplifies complex systems by breaking them into smaller, understandable units.
2. Enhances security by exposing only necessary components.
3. Improves code maintenance and readability.

### (b) Encapsulation
**Encapsulation** is the bundling of data and methods that operate on that data within a single unit, or class. It restricts direct access to some of an object's components, which can prevent unintended interference and misuse.

### (c) Virtual Base Class
A **virtual base class** is used in C++ to prevent multiple instances of a base class appearing in the inheritance hierarchy when using multiple inheritances. It ensures that only one copy of a base class is inherited, avoiding ambiguity and redundancy.

**When to use**: It is useful when we have a "diamond problem" where a base class is inherited multiple times through different paths.

### (d) Polymorphism and Its Types
**Polymorphism** allows objects to be treated as instances of their parent class, enabling a single function or method to work with different types. It comes in two forms:
1. **Compile-time (Static) Polymorphism**: Achieved through function overloading or operator overloading.
2. **Run-time (Dynamic) Polymorphism**: Achieved through inheritance and virtual functions.

Here are the updated C++ examples with `using namespace std;` included:

### (a) Benefits of Data Abstraction

**Example in C++**:
```cpp
#include <iostream>
using namespace std;

class AbstractExample {
public:
    virtual void show() = 0; // Pure virtual function
};

class ConcreteExample : public AbstractExample {
public:
    void show() override { cout << "Data Abstraction Example"; }
};

int main() {
    ConcreteExample obj;
    obj.show();
    return 0;
}
```

### (b) Encapsulation

**Example in C++**:
```cpp
#include <iostream>
using namespace std;

class Encapsulate {
private:
    int data; // private data member
public:
    void setData(int d) { data = d; }  // setter method
    int getData() { return data; }     // getter method
};

int main() {
    Encapsulate obj;
    obj.setData(5);
    cout << obj.getData();
    return 0;
}
```

### (c) Virtual Base Class

**Example in C++**:
```cpp
#include <iostream>
using namespace std;

class Base {
public:
    void show() { cout << "Base class"; }
};

class Derived1 : virtual public Base {};
class Derived2 : virtual public Base {};
class Derived3 : public Derived1, public Derived2 {};

int main() {
    Derived3 obj;
    obj.show(); // No ambiguity due to virtual base class
    return 0;
}
```

### (d) Polymorphism and Its Types

**Example of Compile-time Polymorphism in C++**:
```cpp
#include <iostream>
using namespace std;

class PolymorphismExample {
public:
    void show(int a) { cout << "Integer: " << a; } // Overloaded function
    void show(double a) { cout << "Double: " << a; } // Overloaded function
};

int main() {
    PolymorphismExample obj;
    obj.show(5);    // Calls first version
    obj.show(5.5);  // Calls second version
    return 0;
}
```

**Example of Run-time Polymorphism in C++**:
```cpp
#include <iostream>
using namespace std;

class Base {
public:
    virtual void show() { cout << "Base class"; } // Virtual function
};

class Derived : public Base {
public:
    void show() override { cout << "Derived class"; }
};

int main() {
    Base* ptr;
    Derived obj;
    ptr = &obj;
    ptr->show();  // Calls Derived class's function due to polymorphism
    return 0;
}
```

### 14) What is inline function? When will you make a function inline and why ?

Ans - An **inline function** is a function where the compiler replaces the function call with the actual code of the function, reducing function call overhead.

You'd make a function inline when:
- It's small and called frequently.
- You want to avoid the overhead of function calls.
However, making large functions inline can increase code size and reduce cache efficiency. Use inline for performance-critical, small functions.

### 15) What is a pure virtual function ? Explain use of pure virtual function with an example.

Ans - A **pure virtual function** is a function declared in a base class that has no implementation and must be overridden by derived classes. It is used to create abstract classes, which cannot be instantiated and are meant to be used as base classes.

## Example:
```cpp
class Shape {
public:
    virtual void draw() = 0;  // Pure virtual function
};

class Circle : public Shape {
public:
    void draw() override {
        // Implementation for drawing a circle
    }
};

class Rectangle : public Shape {
public:
    void draw() override {
        // Implementation for drawing a rectangle
    }
};
```
### 16) Explain the concept of default constructor, copy constructor and parameterized constructor with the help of suitable c++ program.

Ans - 
## 1. **Default Constructor**: 
A constructor that takes no parameters and is used to initialize an object with default values.

## 2. **Copy Constructor**: 
A constructor that creates a new object as a copy of an existing object. It takes a reference to another object of the same class as a parameter.

## 3. **Parameterized Constructor**: 
A constructor that takes parameters to initialize an object with specific values.

### Example Program:

```cpp
#include <iostream>
using namespace std;

class Demo {
    int x, y;

public:
    // Default constructor
    Demo() {
        x = 0;
        y = 0;
        cout << "Default Constructor called" << endl;
    }

    // Parameterized constructor
    Demo(int a, int b) {
        x = a;
        y = b;
        cout << "Parameterized Constructor called" << endl;
    }

    // Copy constructor
    Demo(const Demo &obj) {
        x = obj.x;
        y = obj.y;
        cout << "Copy Constructor called" << endl;
    }

    void display() {
        cout << "x: " << x << ", y: " << y << endl;
    }
};

int main() {
    Demo obj1;               // Default constructor
    obj1.display();

    Demo obj2(10, 20);       // Parameterized constructor
    obj2.display();

    Demo obj3 = obj2;        // Copy constructor
    obj3.display();

    return 0;
}
```

### Output:
```
Default Constructor called
x: 0, y: 0
Parameterized Constructor called
x: 10, y: 20
Copy Constructor called
x: 10, y: 20
```
### 17) What is an exception? Explain how exceptions are handled in C++, with the help of an example program. When do we used multiple catch handlers?

Ans- 

An **exception** is an error or unexpected event that occurs during the execution of a program. C++ provides a way to handle exceptions using `try`, `throw`, and `catch` blocks, allowing the program to catch errors and recover instead of terminating abruptly.

## Exception Handling in C++:
- **try**: Code that might throw an exception is placed in the `try` block.
- **throw**: When an error occurs, an exception is thrown using the `throw` keyword.
- **catch**: The `catch` block catches and handles the thrown exception.

## Example Program:
```cpp
#include <iostream>
using namespace std;

int divide(int a, int b) {
    if (b == 0) {
        throw "Division by zero error!";  // Throwing an exception
    }
    return a / b;
}

int main() {
    int x = 10, y = 0;
    
    try {
        cout << "Result: " << divide(x, y) << endl;
    } catch (const char* e) {
        // Catching and handling the exception
        cout << "Exception: " << e << endl;
    }
    
    return 0;
}
```

## Output:
```
Exception: Division by zero error!
```

In this example, the `divide()` function throws an exception when division by zero is attempted, and the `catch` block handles the error.

## Multiple Catch Handlers:
Multiple `catch` blocks can be used to handle different types of exceptions. This is useful when different exceptions need to be handled differently.

## Example with Multiple Catch Blocks:
```cpp
#include <iostream>
using namespace std;

int divide(int a, int b) {
    if (b == 0) throw "Division by zero error!";  // Throw string error
    if (a < 0 || b < 0) throw -1;                // Throw integer error
    return a / b;
}

int main() {
    int x = -10, y = 0;
    
    try {
        cout << "Result: " << divide(x, y) << endl;
    } catch (const char* e) {
        cout << "String Exception: " << e << endl;
    } catch (int e) {
        cout << "Integer Exception: Error code " << e << endl;
    }
    
    return 0;
}
```

## Output:
```
String Exception: Division by zero error!
```

## When to Use Multiple Catch Handlers:
You use multiple catch blocks when:
- You want to handle different types of exceptions differently (e.g., integer, string, object types).
- Different exceptions require different logic to handle them properly.

### 18) What is generic programming? How is it implemented in c++?

Ans - **Generic programming** is a programming paradigm that allows writing code that works with any data type. Instead of writing separate code for each data type, you can write a single, reusable piece of code that operates on various data types. In C++, this is achieved using **templates**.

## Templates in C++:
Templates allow you to define functions or classes that can work with any type of data. There are two types of templates:
1. **Function templates** 
2. **Class templates**

## 1. Function Templates:
A **function template** defines a template for a function, allowing the function to operate on different types of data.

## Example:
```cpp
#include <iostream>
using namespace std;

// Function template for swapping two values
template <typename T>
void swapValues(T& a, T& b) {
    T temp = a;
    a = b;
    b = temp;
}

int main() {
    int x = 5, y = 10;
    double a = 1.5, b = 2.5;

    cout << "Before swap: x = " << x << ", y = " << y << endl;
    swapValues(x, y);  // Swapping integers
    cout << "After swap: x = " << x << ", y = " << y << endl;

    cout << "Before swap: a = " << a << ", b = " << b << endl;
    swapValues(a, b);  // Swapping doubles
    cout << "After swap: a = " << a << ", b = " << b << endl;

    return 0;
}
```

### Output:
```
Before swap: x = 5, y = 10
After swap: x = 10, y = 5
Before swap: a = 1.5, b = 2.5
After swap: a = 2.5, b = 1.5
```

In this example, `swapValues` is a template function that works for any data type (`int`, `double`, etc.) without rewriting the function for each type.

### 2. Class Templates:
A **class template** allows a class to handle different data types. The class definition can use a generic type that will be replaced by the actual type when the object is instantiated.

### Example:
```cpp
#include <iostream>
using namespace std;

// Class template
template <typename T>
class Box {
    T value;
    
public:
    Box(T v) : value(v) {}  // Parameterized constructor

    void display() {
        cout << "Value: " << value << endl;
    }
};

int main() {
    Box<int> intBox(123);    // Box for integers
    intBox.display();

    Box<double> doubleBox(45.67);  // Box for doubles
    doubleBox.display();

    return 0;
}
```

## Output:
```
Value: 123
Value: 45.67
```

In this example, the `Box` class template can handle both `int` and `double` types.

## Benefits of Generic Programming:
- **Code Reusability**: You write a single template function or class that works with multiple data types.
- **Type Safety**: Ensures that type checks are done during compilation, reducing runtime errors.
- **Efficiency**: Templates are resolved at compile-time, meaning there's no runtime overhead.

Generic programming in C++ provides flexibility and reusability while maintaining type safety, making it a powerful feature in the language.

### 19) Distinguish between the term class template and template class.

Ans - Here's a distinction between **class template** and **template class** presented in a chart:

| **Criteria**           | **Class Template**                                        | **Template Class**                                     |
|------------------------|-----------------------------------------------------------|--------------------------------------------------------|
| **Definition**          | A blueprint for creating classes that can handle multiple data types. | A class that is instantiated from a class template with a specific type. |
| **Purpose**             | Used to define generic classes that can work with any data type. | Refers to a class that has already been instantiated from the class template. |
| **Declaration**         | Declared using the `template` keyword with a generic type. Example: `template <typename T> class Box {}` | A specific instantiation of a class template with a concrete data type. Example: `Box<int> myBox;` |
| **Generic**             | It is a template and doesn't represent a specific class until it is instantiated. | Represents a specific type once the class template is instantiated with a concrete type. |
| **Example (Code)**      | `template <typename T> class Box { T value; }`            | `Box<int> intBox;` or `Box<double> doubleBox;`         |
| **When used**           | When defining a class that should support multiple types. | When using a class with a specific data type based on a class template. |
| **Usage**               | Allows for defining classes without specifying a concrete data type. | Refers to the actual class generated from the template for a specific type. |
| **Flexibility**         | More flexible, as it is generic and reusable across types. | Less flexible, as it is specific to the type used during instantiation. |

### 20) Distinguish between overloaded functions and function templates. Write a function template for finding the minimum value contained in an array.

Ans - Here's a distinction between **overloaded functions** and **function templates** presented in a chart:

| **Criteria**             | **Overloaded Functions**                                     | **Function Templates**                                        |
|--------------------------|--------------------------------------------------------------|---------------------------------------------------------------|
| **Definition**            | Multiple functions with the same name but different parameter types. | A single function definition that works with any data type.    |
| **Number of Implementations** | Multiple function implementations, each for different types. | One implementation that is type-independent.                   |
| **Code Reusability**      | Limited, requires writing a new function for each type.       | High, one function works for any type without rewriting.        |
| **Compilation**           | Each overloaded function is compiled separately for each type. | The template is compiled only when instantiated with a specific type. |
| **Ease of Maintenance**   | More difficult to maintain, as each overload needs to be modified. | Easier to maintain, since only one template needs modification. |
| **Flexibility**           | Limited, as specific overloads are needed for each type.      | Highly flexible, automatically works with any type.             |
| **Example (Code)**        | ```void print(int x); void print(double x);```                | ```template <typename T> void print(T x);```                    |

## Example of a Function Template for Finding the Minimum Value in an Array:

```cpp
#include <iostream>
using namespace std;

// Function template to find the minimum value in an array
template <typename T>
T findMin(T arr[], int size) {
    T min = arr[0];
    for (int i = 1; i < size; i++) {
        if (arr[i] < min)
            min = arr[i];
    }
    return min;
}

int main() {
    int intArr[] = {3, 1, 4, 1, 5};
    double doubleArr[] = {2.5, 3.1, 0.9, 4.0};

    cout << "Min in intArr: " << findMin(intArr, 5) << endl;     // Works for int
    cout << "Min in doubleArr: " << findMin(doubleArr, 4) << endl;  // Works for double

    return 0;
}
```

## Output:
```
Min in intArr: 1
Min in doubleArr: 0.9
```

In this template, `findMin()` works with arrays of any data type (`int`, `double`, etc.), demonstrating how templates avoid the need for separate function overloads.
