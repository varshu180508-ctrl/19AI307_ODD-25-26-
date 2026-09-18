# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
Construct a right-angled triangle star pattern using for loop.
## AIM:
To write a Java program using looping statements to print a right-angled triangle star pattern based on user input.

## ALGORITHM :
1.	Start the program.

2.	Import the necessary package 'java.util'

3. Read the number of rows from the user.

4. Use an outer loop to iterate through each row.

5. Use an inner loop to print stars (*) for each row.

6. Move to the next line after printing stars for each row.

7. End the program.


## PROGRAM:
<h2 align="center">
  🔄 <b>Program to Implement a Looping Statement Using Java</b>
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
  📚 <b>Topic:</b> Looping Statements
</p>


## SOURCE CODE:

```
import java.util.*;
public class TrianglePattern
{
    public static void main(String args[])
    {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        for (int i = 1; i <= n; i++) 
        {         
            for (int j = 1; j <= i; j++) 
            {      
                System.out.print("* ");
            }
            System.out.println();              
        }
    }
}
```




## OUTPUT:
<img width="492" height="492" alt="image" src="https://github.com/user-attachments/assets/0e0897d4-fe47-4780-b561-a911cb8e667e" />




## RESULT:
Thus, the Java program using looping statements to print a right-angled triangle star pattern was successfully written, executed, and verified.
