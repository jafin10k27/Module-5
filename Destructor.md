# Exp.No:22  
## Destructor:Create a Python  class Vehicle that  has a constructor (init) and destructor (del). We create an instance from the class and delete it right after.

### AIM  
To write a Python program to demonstrate the use of a constructor (__init__) and a destructor (__del__) in a class.

### ALGORITHM

1.Define a class named Vehicle.

2.Create a constructor method __init__() inside the class that prints "Vehicle created.".

3.Create a destructor method __del__() inside the class that prints "Destructor called, vehicle deleted.".

4.Create an object of the Vehicle class.

5.This will automatically call the constructor.

6.Delete the object using the del statement.

7.This will automatically call the destructor.

### PROGRAM

```
# Reg.No-212223020018
# Name-Mohamed Jafin S
class Vehicle:
    def __init__(self):
        print('Vehicle created.')

    def __del__(self):
        print('Destructor called, vehicle deleted.')

car = Vehicle() # this is where the object is created and the constructor is called
del car

```

### OUTPUT
![image](https://github.com/user-attachments/assets/90fc58ea-cf0e-406e-8692-389ca80a472e)

### RESULT
Result
The constructor is invoked when the object car is created, displaying the message:
"Vehicle created."

The destructor is invoked when the object car is deleted, displaying the message:
"Destructor called, vehicle deleted."
