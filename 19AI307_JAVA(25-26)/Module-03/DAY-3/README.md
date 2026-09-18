# Ex.No:3(C) ABSTRACTION

## QUESTION:

Create an abstract class **TaxPayer** with an abstract method `calculateTax()`.
Create two subclasses **SalariedPerson** and **BusinessPerson**, each implementing their respective tax calculation logic.

## AIM:

To write a Java program that demonstrates **abstraction** using an abstract class and method, implemented differently in subclasses for tax calculation.

## ALGORITHM :

1. Start the program.
2. Import the necessary package `java.util`.
3. Create an abstract class `TaxPayer` with an abstract method `calculateTax()`.
4. Create subclasses `SalariedPerson` and `BusinessPerson` that override `calculateTax()` with specific tax rules.
5. Read taxpayer type and income from the user.
6. Use conditional logic to create the appropriate subclass object.
7. Call `calculateTax()` and print the tax.
8. Stop the program.

## PROGRAM:

<h2 align="center">  
  🎭 <b>Program to Implement Abstraction Using Java</b>  
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
  📚 <b>Topic:</b> Abstraction  
</p>

## SOURCE CODE:

```java
import java.util.*;

abstract class TaxPayer {
    double income;
    TaxPayer(double income) {
        this.income = income;
    }
    abstract double calculateTax();
}

class SalariedPerson extends TaxPayer {
    SalariedPerson(double income) {
        super(income);
    }
    double calculateTax() {
        return income * 0.10;
    }
}

class BusinessPerson extends TaxPayer {
    BusinessPerson(double income) {
        super(income);
    }
    double calculateTax() {
        return income * 0.15;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int type = sc.nextInt();
        double income = sc.nextDouble();
        TaxPayer p = (type == 1) ? new SalariedPerson(income) : new BusinessPerson(income);
        System.out.printf("%.2f\n", p.calculateTax());
    }
}
```

## OUTPUT:
<img width="617" height="472" alt="image" src="https://github.com/user-attachments/assets/18fd736a-a317-40b8-96b4-6f5515536824" />



## RESULT:

Thus, the Java program implementing **abstraction** using an abstract class TaxPayer and its subclasses was successfully executed.
