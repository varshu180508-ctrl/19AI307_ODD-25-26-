# Ex.No:4(A) EXCEPTION HANDLING

## QUESTION:

You are writing a Java program where you read a string input. If the input is "init", you create an object and call its method. If it's "null", no object is created. Your program crashes with a NullPointerException when "null" is entered.

## AIM:

To write a Java program that demonstrates exception handling by catching a NullPointerException when an object is not initialized.

## ALGORITHM :

1. Start the program.
2. Import the necessary package 'java.util'.
3. Read a string input from the user.
4. Declare an object reference and assign it null.
5. Create an object only if the user enters "init".
6. Attempt to call a method inside a try block.
7. Catch NullPointerException and display an appropriate message.
8. End the program.

## PROGRAM:

<h2 align="center">  
  ⚠️ <b>Program to Implement Exception Handling Using Java</b>  
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
  📚 <b>Topic:</b> Exception Handling  
</p>


## SOURCE CODE:

```java
import java.util.Scanner;

class Example {
    void display() {
        System.out.println("Object exists");
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String str = sc.nextLine();
        
        Example ex = null;

        if(str.equalsIgnoreCase("init")) {
            ex = new Example();
        } 
        
        try {
            ex.display();
        } catch (NullPointerException e) {
            System.out.println("Object is null");
        }
    }
}
```

## OUTPUT:
<img width="697" height="248" alt="image" src="https://github.com/user-attachments/assets/c7218592-2d22-4201-86b7-52eb1352a65a" />


## RESULT:

Thus, the Java program to demonstrate exception handling using NullPointerException was successfully implemented.
