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
```
class Details:
    def get_details(self, id, name, gender):
        self.id = id
        self.name = name
        self.gender = gender

class Employee(Details):
    def get_emp(self, company, department):
        self.company = company
        self.department = department

    def display_emp(self):
        print("Employee Object")
        print("Id: ", self.id)
        print("Name: ", self.name)
        print("Gender: ", self.gender)
        print("Company: ", self.company)
        print("Department: ", self.department)
        print()

class Doctor(Details):
    def get_doc(self, hospital, department):
        self.hospital = hospital
        self.department = department

    def display_doc(self):
        print("Doctor Object")
        print("Id: ", self.id)
        print("Name: ", self.name)
        print("Gender: ", self.gender)
        print("Hospital: ", self.hospital)
        print("Department: ", self.department)

# Main program
# Employee details
id1 = int(input())
name1 = input()
gender1 = input()
company = input()
department1 = input()

# Doctor details
id2 = int(input())
name2 = input()
gender2 = input()
hospital = input()
department2 = input()

emp = Employee()
emp.get_details(id1, name1, gender1)
emp.get_emp(company, department1)

doc = Doctor()
doc.get_details(id2, name2, gender2)
doc.get_doc(hospital, department2)

emp.display_emp()
doc.display_doc()
```
## Sample Output
<img width="1176" height="481" alt="image" src="https://github.com/user-attachments/assets/90a80217-1593-4ea8-bf39-2034f2437762" />

Result 
The program is executed


