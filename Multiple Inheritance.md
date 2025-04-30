# Exp.No:23  
## Multiple Inheritance:Write A Python Program to Calculated Add,  Mul and division using Multiple Inheritance.

### AIM  
To write a Python program to perform addition, multiplication, and division using multiple inheritance.

### ALGORITHM
1.Create a class Calculation1:
Define a method Summation(a, b) that returns the sum of two numbers.

2.Create another class Calculation2:
Define a method Multiplication(a, b) that returns the product of two numbers.

3.Create a derived class Derived that inherits from both Calculation1 and Calculation2:
Define a method Divide(a, b) that returns the division of two numbers.

4.Accept two integers as input from the user.

5.Create an object of the Derived class.

6.Call the methods Summation, Multiplication, and Divide using the object and display the results.

### PROGRAM

```
# Reg.No-212223020018
# Name-Mohamed Jafin S
class Calculation1:
    def Summation(self,a,b):
        return a+b;
class Calculation2:
    def Multiplication(self,a,b):
        return a*b;
class Derived(Calculation1,Calculation2):
    def Divide(self,a,b):
        return a/b;

a=int(input())
b=int(input())
d=Derived()
print(d.Summation(a,b))
print(d.Multiplication(a,b))
print(d.Divide(a,b))
```

### OUTPUT
![image](https://github.com/user-attachments/assets/d41941f2-c9c6-49df-875f-25edf2186e6a)


### RESULT
The program successfully performs addition, multiplication, and division using multiple inheritance.

It displays the correct output for the given input numbers.
