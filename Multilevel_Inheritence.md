# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
class Person:
    def get_name(self):
        self.name = input("Enter Name: ")

class Age(Person):
    def get_age(self):
        self.age = int(input("Enter Age: "))

class Location(Age):
    def get_location(self):
        self.location = input("Enter Location: ")

    def display(self):
        print("\n--- Person Details ---")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Location:", self.location)

obj = Location()

obj.get_name()
obj.get_age()
obj.get_location()

obj.display()

## Sample Output
Enter Name: Ravi
Enter Age: 22
Enter Location: Chennai

--- Person Details ---
Name: Ravi
Age: 22
Location: Chennai

##Result
The program successfully demonstrates Multilevel Inheritance in Python. The Location class inherits properties and methods from both the Age and Person classes, allowing it to collect and display the person's name, age, and location through a multilevel inheritance structure.
