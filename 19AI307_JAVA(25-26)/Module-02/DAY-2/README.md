# Ex.No:2(B) METHODS

## QUESTION:

Create two methods:

1. **double getArea(double r)** → Calculates and returns the area of a circle (should not print anything).
2. **void printArea(double area)** → Prints the calculated area.

The program reads the radius from the user, computes the area using `getArea()`, and prints it using `printArea()`.

Example:

| Input | Result |
| ----- | ------ |
| 2     | 12.56  |

---

## AIM:

To write a Java program that demonstrates the use of methods by calculating and printing the area of a circle using separate functions for computation and output.

---

## ALGORITHM :

1. Start the program.
2. Import the necessary package `java.util`.
3. Define a method `getArea()` to calculate and return the area of a circle.
4. Define a method `printArea()` to print the area passed to it.
5. In the main method, get user input for radius.
6. Call `getArea()` to compute the area.
7. Call `printArea()` to display the area.
8. End the program.

---

## PROGRAM:

<h2 align="center"> 
  ⚙️ <b>Program to Implement Methods Using Java</b> 
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
  📚 <b>Topic:</b> Methods 
</p>

---

## SOURCE CODE:

```java
import java.util.*;
class prog {
    double getArea(double r) {
        return 3.14*r*r;
    }
    void printArea(double area) {
        System.out.printf("%.2f",area);
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        prog obj = new prog();
        double r = sc.nextDouble();
        obj.printArea(obj.getArea(r));
    }
}
```

---

## OUTPUT:
<img width="543" height="267" alt="image" src="https://github.com/user-attachments/assets/29664057-a7e2-415f-ba2e-3f3a507e3cb0" />



---

## RESULT:

Thus, the Java program using methods to compute and display the area of a circle was successfully executed and the output was verified.
