
# Exp.No:21  
## Constructors -Write a python program using class to perform addition of two numbers using parameterised constructor.

### AIM  
To write a Python program using a class with a parameterized constructor to perform the addition of two numbers.

### ALGORITHM

1.Define a class named Addition.

2.Declare three attributes inside the class: first, second, and answer, initializing them to 0.

3.Create a parameterized constructor __init__() that accepts two arguments and assigns them to first and second4..

4.Create a calculate() method that adds the two numbers and stores the result in answer.

5.Create a display() method that prints the values of first, second, and answer.

6.Take two numbers as input from the user.

7.Create an object of the Addition class by passing the two numbers to the constructor.

8.Call the calculate() method to perform the addition.

9.Call the display() method to show the result.


### PROGRAM

```
# Reg.No-212223020018
# Name-Mohamed Jafin S
class Addition:
    first = 0
    second = 0
    answer = 0
     
    # parameterized constructor
    def __init__(self, f, s):
        self.first = f
        self.second = s
     
    def display(self):
        print("First number = " + str(self.first))
        print("Second number = " + str(self.second))
        print("Addition of two numbers = " + str(self.answer))
 
    def calculate(self):
        self.answer = self.first + self.second
 
# creating object of the class
# this will invoke parameterized constructor
x=int(input())
y=int(input())

obj = Addition(x,y)
 
# perform Addition
obj.calculate()
 
# display result
obj.display()

```

### OUTPUT
![image](https://github.com/user-attachments/assets/f4ccacc5-ecf9-4b6e-b83e-3ba5de83940a)

### RESULT
The program successfully accepts two numbers from the user.

It calculates their sum using a class with a parameterized constructor.

It displays the first number, second number, and their addition result.
