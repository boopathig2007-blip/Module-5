# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
class Details:
    def get_details(self):
        self.name = input("Enter Name: ")
        self.age = int(input("Enter Age: "))

class Employee(Details):
    def get_employee(self):
        self.emp_id = input("Enter Employee ID: ")
        self.department = input("Enter Department: ")

    def display_employee(self):
        print("\n--- Employee Details ---")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Employee ID:", self.emp_id)
        print("Department:", self.department)

class Patient(Details):
    def get_patient(self):
        self.patient_id = input("Enter Patient ID: ")
        self.disease = input("Enter Disease: ")

    def display_patient(self):
        print("\n--- Patient Details ---")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Patient ID:", self.patient_id)
        print("Disease:", self.disease)

# Employee Details
e = Employee()
e.get_details()
e.get_employee()
e.display_employee()

# Patient Details
p = Patient()
p.get_details()
p.get_patient()
p.display_patient()

## Sample Output
Enter Name: Raj
Enter Age: 30
Enter Employee ID: E101
Enter Department: IT

--- Employee Details ---
Name: Raj
Age: 30
Employee ID: E101
Department: IT

Enter Name: Kumar
Enter Age: 45
Enter Patient ID: P201
Enter Disease: Fever

--- Patient Details ---
Name: Kumar
Age: 45
Patient ID: P201
Disease: Fe 

Result
The program successfully demonstrates Hierarchical Inheritance in Python, where the classes Employee and Patient inherit common attributes and methods from the parent class Details while maintaining their own specific properties and functionalities.

