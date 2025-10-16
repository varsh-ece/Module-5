# # Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student’s name provided by the user.

## 🧠 Algorithm
1. **Get user input**: Accept the student's name from the user.
2. **Define the class**: Create a class `Student` with a default constructor (`__init__`).
3. **Default Constructor**: In the constructor, assign the user input (student name) to an instance variable `self.a`.
4. **Display Message**: Define a method `show` that prints "This is non-parameterized constructor" and a welcome message with the student’s name.
5. **Execute the Program**: Instantiate the `Student` class and call the `show` method.

## 🧾 Program
~~~
class student:
    def __init__(self):
        print("This is non parametrized constructor")
    def display_welcome(self,name):
        print(f"Hello {name}")
name=input()
studentinstance=student()
studentinstance.display_welcome(name)
~~~

## Output
<img width="838" height="220" alt="image" src="https://github.com/user-attachments/assets/45adc714-ae27-4e3a-bb64-85338bbb11c5" />


## Result
Thus the output is Verified.

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
~~~
class Demo:
    def __init__(self):
        print ("Alive")
    def __del__(self):
        print("The object no longer exists")
obj=Demo()
~~~

## 🧪 Output
<img width="595" height="163" alt="image" src="https://github.com/user-attachments/assets/45257350-6528-45f1-bd76-344cd37d6330" />


## Result
Thus the output is verified.

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
~~~
# Single inheritance in python
#Base class
class Details(object): 
# Constructor 
    def __init__(self, name, id): 
        self.name = name 
        self.id = id
# To fetch employee details 
    def Employee_Details(self): 
        return self.id , self.name
# derived class or the sub class
class Patient_details(Employee_details): 
    # To check if this  is a valid employee 
    def Employee_check(self): 
        if self.id > 500000:
           return " Valid Employee "
        else:
           return " Invalid Employee "
# Driver code 
id=int(input())
name=input()
Employee1 = Patient_details( name , id)  # parent class object
print( Employee1.Employee_Details() , Employee1.Employee_check() ) 
~~~
## Sample Output
<img width="811" height="229" alt="image" src="https://github.com/user-attachments/assets/c7ce9114-9cc3-4586-a672-1f749b467d4d" />

## Result
Thus the output is verified.

