# Ex.No:4(B)  IMPLEMENT SOLID PRINCIPLES IN JAVA PROGRAM

## QUESTION:

In a large office, multiple departments send print jobs to a shared central printer. To manage load and prevent collision, a Print Spooler Manager handles all job submissions.

The IT team insists that there should be only one spooler manager instance in the entire system. Regardless of how many jobs or departments exist, all jobs must pass through this one manager.

Your task is to simulate a singleton print job queue. Each print job submitted increases the queue count.

Hidden Clue:
Use Singleton to manage shared access.

Count and log each print job submission.

Validate that state is preserved across all accesses.

Input Format:
First line: Integer n – number of print jobs

Next n lines: Each line contains the department name submitting the print job.

Output Format:
For each job, print:

## AIM:

To implement the Singleton Design Pattern ensuring that only one Print Spooler Manager instance handles all print jobs.

## ALGORITHM :

1. Start the program.
2. Import the necessary package `java.util`.
3. Create a class with a private static instance and private constructor.
4. Provide a public static method to return the singleton instance.
5. Maintain a print job counter inside the singleton class.
6. Read the number of print jobs from the user.
7. For each department input, access the singleton instance and update the job count.
8. Display the total print job count after each submission.
9. End the program.

## PROGRAM:

<h2 align="center">  
  🧩 <b>Program to Implement SOLID Principles in Java</b>  
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
  📚 <b>Topic:</b> SOLID Principles  
</p>


## SOURCE CODE:

```java
import java.util.*;

class PrintSpoolerManager {
    private static PrintSpoolerManager instance;
    private int count = 0;

    public static PrintSpoolerManager getInstance() {
        if(instance == null) {
            instance = new PrintSpoolerManager();
        }
        return instance;
    }

    public int submitJob(String department) {
        return ++count;
    }
}

public class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) {
            String dept = sc.nextLine();
            PrintSpoolerManager spooler = PrintSpoolerManager.getInstance();
            int total = spooler.submitJob(dept);
            System.out.println(dept + " submitted a print job. Total Jobs in Queue: " + total);
        }
    }
}
```

## OUTPUT:
<img width="1246" height="390" alt="image" src="https://github.com/user-attachments/assets/7b608518-ad85-42fe-a64b-a1e6e3fb8bb0" />


## RESULT:

Thus, the Java program implementing the Singleton principle for a shared print spooler manager was successfully executed.
