# Ex.No:5(D) THREAD PRIORITY

## QUESTION:

Write a java program for set the priority and name of the current thread.

Note : Read the threadname from the User

Set the Priority as 2.

### Input / Output Format:

| Input     | Result                                                                         |
| --------- | ------------------------------------------------------------------------------ |
| NewThread | Priority of Thread: 2<br>Name of Thread: NewThread<br>Thread[NewThread,2,main] |

## AIM:

To write a Java program that reads a thread name from the user, assigns it to the current thread, sets its priority to 2, and displays the updated thread details.

## ALGORITHM :

1. Start the program.
2. Import the necessary package `java.util`.
3. Read the thread name from the user.
4. Get the current executing thread.
5. Set the thread’s name and priority to 2.
6. Display the thread priority, name, and thread details.
7. Stop the program.

## PROGRAM:
<h2 align="center">  
  🧵 <b>Program to Implement Thread Name and Priority Using Java</b>  
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
  📚 <b>Topic:</b> Thread Name and Priority  
</p>



## SOURCE CODE:

```java
import java.util.Scanner;
public class Main{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String threadName = sc.nextLine();

        Thread t = Thread.currentThread();
        t.setName(threadName);
        t.setPriority(2);

        System.out.println("Priority of Thread: " + t.getPriority());
        System.out.println("Name of Thread: " + t.getName());
        System.out.println(t);
    }
}
```

## OUTPUT:

<img width="847" height="320" alt="image" src="https://github.com/user-attachments/assets/0fb5fb87-ff20-40af-9266-9ee5d9d20c65" />


## RESULT:

Thus, the Java program to set and display the priority and name of the current thread was successfully executed.
