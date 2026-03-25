# Destructor in Python

This project demonstrates how to implement a **destructor** in Python using a simple class.

## 🚀 Overview

The program defines a class `Demo` with:

- A **constructor** `__init__` that initializes an instance variable and prints a message.
- A **destructor** `__del__` that prints a message when the object is destroyed.

## 🧠 Algorithm

1. Define a class named `Demo`.
2. Inside the class, define the `__init__` method:
   - Initialize an instance variable `status` with the value `"Alive"`.
   - Print the value of `status`.
3. Define the `__del__` method:
   - Print a message indicating the object is being destroyed.
4. Outside the class:
   - Create an instance of the `Demo` class.
   - Delete the object using the `del` keyword.
## Program
```
class Demo:
  
    def __init__(self):
      
        self.status = "Alive"
        print(f"Object created. Status: {self.status}")

    def __del__(self):
        print("Destructor called, object is being destroyed.")
 Outside the class:

obj = Demo()
```
## 🧪 Output
Object created. Status: Alive
Destructor called, object is being destroyed.

## Result
The __init__ method is automatically called when the object obj is instantiated, setting the status to "Alive".
The __del__ method is triggered when the del keyword is used, effectively cleaning up the object and printing the destruction message.

