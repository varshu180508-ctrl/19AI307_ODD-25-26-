# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:

Write a Java program to demonstrate a parameterized constructor.

## AIM:

To write a Java program that demonstrates the use of a parameterized constructor to initialize object values.

## ALGORITHM :

1. Start the program.
2. Import the necessary package `java.util`.
3. Create a class `Employee` with variables `name` and `id`.
4. Define a parameterized constructor to initialize the variables.
5. Create a method `display()` to print the employee details.
6. In the `main` method, create a `Scanner` object to read user input.
7. Create an `Employee` object by passing the input values to the parameterized constructor.
8. Call the `display()` method to print the output.
9. End the program.

## PROGRAM:

<h2 align="center">  
  🔧 <b>Program to Implement Variable Scope and Constructor Using Java</b>  
</h2>  

<p align="center">  
  👨‍💻 <b>Developed By:</b><br>  
  <b>DHANVARSINI S</b>  
  <br><br>  
  🆔 <b>Register Number:</b><br>  
  <b>212225240032</b>  
</p>  

<hr>  

<p align="center">  
  📌 <b>Language:</b> Java<br>  
  📚 <b>Topic:</b> Variable Scope and Constructor  
</p>


## SOURCE CODE:

```java
import java.util.*;

class Employee {
    String name;
    int id;

    Employee(String name, int id) {
        this.name = name;
        this.id = id;
    }

    void display() {
        System.out.println("Employee Name: " + name);
        System.out.println("Employee ID: " + id);
    }
}

class prog {
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);
        Employee obj = new Employee(sc.nextLine(), sc.nextInt());
        obj.display();
    }
}
```

## OUTPUT:
<img width="702" height="396" alt="image" src="https://github.com/user-attachments/assets/035f34d1-d410-4594-9ccf-18aaab824934" />



## RESULT:

Thus, the Java program to demonstrate a parameterized constructor was successfully executed.

---

