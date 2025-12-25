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
```
class Add:
    def addition(self, a, b):
        return a + b

class Sub:
    def subtraction(self, a, b):
        return a - b

class Div(Add, Sub):
    def division(self, a, b):
        return a / b

# Main program
a = int(input())
b = int(input())

obj = Div()

print(obj.addition(a, b))
print(obj.subtraction(a, b))
print(obj.division(a, b))
```
## Output Example
<img width="1150" height="217" alt="image" src="https://github.com/user-attachments/assets/fea43a72-9134-45d1-a387-eb67ae44bb3b" />

The program is executed

