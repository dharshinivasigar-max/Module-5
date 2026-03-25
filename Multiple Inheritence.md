# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 
~~~
class Calculation1:
    def Summation(self, a, b):
        return a + b

class Calculation2:
    def Subtraction(self, a, b):
        return a - b

class Derived(Calculation1, Calculation2):
    def Division(self, a, b):
        return a / b

num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))

d = Derived()

print("Sum:", d.Summation(num1, num2))
print("Difference:", d.Subtraction(num1, num2))
print("Division:", d.Division(num1, num2))
~~~
## Output Example
This program illustrates multiple inheritance in Python, where a single class (Derived) inherits attributes and methods from more than one parent class (Calculation1 and Calculation2). By creating an object of the Derived class, we gain access to the Summation and Subtraction methods from the base classes, as well as the Division method defined within the child class itself.
