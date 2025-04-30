# Exp.No:25  
## Hierarchical Inheritance:Write a Python program to Get the employee  and patient details & display it using Hierarchical inheritance.
## Note: create a parent (base) class name Details and two child (derived) classes named Employee and Patient.

### AIM  
To write a Python program using hierarchical inheritance where a parent class Details is inherited by two child classes Employee and Patient to input and display their respective details.


### ALGORITHM
1.Define a base class Details:

Initialize private attributes id, name, and gender.

Create a setData() method to set the values of these attributes.

Create a showData() method to display these attributes.

2.Define a derived class Employee that inherits from Details:

Add private attributes company and department.

Create a setEmployee() method to set both the personal and employee-specific attributes.

Create a showEmployee() method to display all employee details.

3.Define another derived class Patient that inherits from Details:

Add private attributes hospital and department.

Create a setEmployee() (should be better named setPatient()) method to set personal and patient-specific attributes.

Create a showEmployee() (should be better named showPatient()) method to display all patient details.

4.Take input for both an employee and a patient from the user.

5.Create objects for Employee and Patient.

6.Set and display their respective data using their methods.


### PROGRAM
```
# Reg.No-212223020018
# Name-Mohamed Jafin S
# hierarchical inheritance

class Details:
    def __init__(self):
        self.__id="<No Id>"
        self.__name="<No Name>"
        self.__gender="<No Gender>"
        
    def setData(self,id,name,gender):
        self.__id=id
        self.__name=name
        self.__gender=gender
    def showData(self):
        print("Id: ",self.__id)
        print("Name: ", self.__name)
        print("Gender: ", self.__gender)

class Employee(Details): #Inheritance
    def __init__(self):
        self.__company="<No Company>"
        self.__dept="<No Dept>"
        
    def setEmployee(self,id,name,gender,comp,dept):
        self.setData(id,name,gender)
        self.__company=comp
        self.__dept=dept
    def showEmployee(self):
        self.showData()
        print("Company: ", self.__company)
        print("Department: ", self.__dept)

class Patient(Details): #Inheritance
    def __init__(self):
        self.__hospital="<No Hospital>"
        self.__dept="<No Dept>"
    def setEmployee(self,id,name,gender,hos,dept):
        self.setData(id,name,gender)
        self.__hospital=hos
        self.__dept=dept
    def showEmployee(self):
        self.showData()
        print("Hospital: ", self.__hospital)
        print("Department: ",self.__dept)
        

id=int(input())
name=input()
gender=input()
comp=input()
dept=input()
id1=int(input())
nam=input()
gen=input()
hosp=input()
dep=input()

print("Employee Object")
e=Employee()
e.setEmployee(id,name,gender,comp,dept)
e.showEmployee()
print("\nPatient Object")
d = Patient()
d.setEmployee(id1, nam, gen, hosp, dep)
d.showEmployee()


```

### OUTPUT  
![image](https://github.com/user-attachments/assets/7a51b722-2b65-4e3b-8916-efd4611d792e)



### RESULT
The program successfully implements hierarchical inheritance.
It correctly inputs and displays the details of an employee and a patient separately.
