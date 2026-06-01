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
class Addition:
    def add(self, a, b):
        print("Addition =", a + b)

class Subtraction:
    def subtract(self, a, b):
        print("Subtraction =", a - b)

class Division(Addition, Subtraction):
    def divide(self, a, b):
        if b != 0:
            print("Division =", a / b)
        else:
            print("Division by zero is not possible")

obj = Division()

a = int(input("Enter First Number: "))
b = int(input("Enter Second Number: "))

obj.add(a, b)
obj.subtract(a, b)
obj.divide(a, b)
## Output Example
Enter First Number: 20
Enter Second Number: 5

Addition = 25
Subtraction = 15
Division = 4.0

 Result:
 The program successfully demonstrates Multiple Inheritance in Python. The Division class inherits methods from both Addition and Subtraction classes and performs Addition, Subtraction, and Division operations using a single object.

