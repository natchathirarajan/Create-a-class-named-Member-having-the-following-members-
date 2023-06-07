# Exp-10-Write-a-program-to-print-salary-of-an-employee.

## AIM:
To write a java program to print salary of an employee.

## ALGORITHM: 
### Step 1:
Import the necessary packages.
### Step 2: 
Create a Class named 'Member' which has data members.
### Step 3: 
Add a method printSalary to print the salary in that class.
### Step 4: 
Create two other classes 'Employee' and 'Manager' which inherits 'Member' class.
### Step 5:  
Assign details to an employee and a manager by making an object of both of these classes.
### Step 6:  
Print the result.
### Step 7: 
End the program.
## PROGRAM:

~~~
public class Member {
    private String name;
    private int age;
    private String phoneNumber;
    private String address;
    private double salary;
    public Member(String name, int age, String phoneNumber, String address,
                  double salary) {
        this.name = name;
        this.age = age;
        this.phoneNumber = phoneNumber;
        this.address = address;
        this.salary = salary;
    }
    public void printSalary() {
        System.out.println("Salary :" + salary);
    }
}

public class Employee extends Member {
    private String specialization;
    public Employee(String name, int age, String phoneNumber,
                    String address, double salary, String specialization) {
        super(name, age, phoneNumber, address, salary);
        this.specialization = specialization;
    }
}

public class Manager extends Member{
    private String department;
    public Manager(String name, int age, String phoneNumber,
                   String address, double salary, String department) {
        super(name, age, phoneNumber, address, salary);
        this.department = department;
    }
}

public class Main {
    public static void main(String[] args) {
        Employee employee = new Employee("John", 25, "9856452634", "T.Nagar",
                25000, "IT");
        Manager manager = new Manager("Arjun", 30, "8425631579", "Anna Nagar",
                80000, "AI&ML");

        //Employee Salary
        employee.printSalary();
        //Manager Salary
        manager.printSalary();
    }
}
~~~

## OUTPUT:
![exp10](https://github.com/abdulwasih2003/Exp-10-Write-a-program-to-print-details-of-an-employee/assets/91781810/9d0fb2f5-1756-47bc-9a7e-9f408976ae36)

## RESULT:
Thus the java program to print salary of an employee is successful.

