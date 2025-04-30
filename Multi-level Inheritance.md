
# Exp.No:24  
## Multi-level Inheritance:Write a Python program to Get the name, age and location of a person and display using Multilevel inheritance.

### AIM  
To write a Python program using multilevel inheritance to get and display the name, age, and location of a person.

### ALGORITHM
1.Create a base class Parent:

It should have a constructor that initializes the name.

It should have a method getName() to return the name.

2.Create a derived class Child that inherits from Parent:

It should have a constructor that initializes name (by calling parent constructor) and age.

It should have a method getAge() to return the age.

3.Create another derived class Grandchild that inherits from Child:

It should have a constructor that initializes name, age (by calling child constructor) and location.

It should have a method getLocation() to return the location.

4.Take user input for name, age, and location.

5.Create an object of Grandchild.

6.Display the name, age, and location using the respective methods.

### PROGRAM

```
# Reg.No-212223020018
# Name-Mohamed Jafin S
class Parent:
    def __init__(self,name):
        self.name=name
    def getName(self):
        return self.name
class Child(Parent):
    def __init__(self,name,age):
        Parent.__init__(self,name)
        self.age=age
        
    def getAge(self):
        return self.age
class Grandchild(Child):
    def __init__(self,name,age,location):
        Child.__init__(self,name,age)
        self.location=location
    def getLocation(self):
        return self.location
        
name=input()
age=int(input())
loc=input()
gc=Grandchild(name,age,loc)
print(gc.getName(), gc.getAge(), gc.getLocation())

```

### OUTPUT
![image](https://github.com/user-attachments/assets/d4999515-d718-45d2-a480-e4378de56899)

### RESULT

The program successfully accepts a person's name, age, and location.

It displays the collected information using multilevel inheritance.
