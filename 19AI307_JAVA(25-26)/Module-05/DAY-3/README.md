# Ex.No:5(C)  FILE HANDLING USING JAVA

## QUESTION:

Write a Java program to read a file and print only the lines containing the word **"Java"**.

## AIM:

To write a program that accepts user input, stores it in a file, and displays only the lines that contain the word **"Java"**.

## ALGORITHM :

1. Start the program.
2. Import the necessary packages (`java.io.*`, `java.util.*`).
3. Create a `File` object and a `FileWriter` to write user input into the file.
4. Read user input until the user types `"exit"`.
5. Write each line into the file.
6. After writing, read the file using `BufferedReader`.
7. Print only the lines that contain the word `"Java"`.
8. Close all streams.

---

## PROGRAM:

<h2 align="center">  
  📁 <b>Program to Implement File Handling Using Java</b>  
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
  📚 <b>Topic:</b> File Handling  
</p>


## SOURCE CODE:

```java
import java.io.*;
import java.util.Scanner;

class prog {
    public static void main(String args[]) throws IOException {

        Scanner sc = new Scanner(System.in);
        File file = new File("sample.txt");
        FileWriter writer = new FileWriter(file);

        System.out.println("Enter lines (type 'exit' to stop):");

        while (true) {
            String line = sc.nextLine();
            if (line.equals("exit")) break;
            writer.write(line + "\n");
        }

        writer.close();

        System.out.println("Lines containing the word 'Java':");

        BufferedReader br = new BufferedReader(new FileReader(file));
        String l;

        while ((l = br.readLine()) != null) {
            if (l.contains("Java")) {
                System.out.println(l);
            }
        }

        br.close();
    }
}
```

---

## OUTPUT:

<img width="1111" height="428" alt="image" src="https://github.com/user-attachments/assets/c817016c-3929-428d-b3bb-7e214f157200" />



---

## RESULT:

Thus, the program to read a file and print lines containing the word **"Java"** was successfully executed.
