# Ex.No:4(C)  COMPOSITION IN JAVA

## QUESTION:

Implement a system where a Library contains multiple Book objects. Each Book is created inside the Library. Books can't exist independently (Composition).

### Example

| **Input**                                                | **Result**                                                                   |
| -------------------------------------------------------- | ---------------------------------------------------------------------------- |
| 2<br>Java<br>James Gosling<br>Python<br>Guido Van Rossum | Books in Library:<br>- Java by James Gosling<br>- Python by Guido Van Rossum |
| 1<br>Machine Learning<br>Andrew Ng                       | Books in Library:<br>- Machine Learning by Andrew Ng                         |

## AIM:

To write a Java program that demonstrates Composition by creating Book objects inside a Library class, ensuring Books cannot exist independently and displaying them.

## ALGORITHM :

1. Start the program.
2. Import the necessary package `java.util`.
3. Create a `Book` class with title and author.
4. Create a `Library` class that stores Book objects.
5. Read the number of books, then read book details.
6. Add each book to the Library and display the list.
7. End the program.

## PROGRAM:

<h2 align="center">  
  🧱 <b>Program to Implement Composition Concepts in Java</b>  
</h2>  

<p align="center">  
  👨‍💻 <b>Developed By:</b><br>  
  <b>DHANAVARSINI S</b>  
  <br><br>  
  🆔 <b>Register Number:</b><br>  
  <b>212225240032</b>  
</p>  

<hr>  

<p align="center">  
  📌 <b>Language:</b> Java<br>  
  📚 <b>Topic:</b> Composition Concepts  
</p>

## SOURCE CODE:

```java
import java.util.*;

public class CompositionExample {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Library library = new Library();

        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) {
            String title = sc.nextLine();
            String author = sc.nextLine();
            library.addBook(title, author);
        }

        library.showBooks();
        sc.close();
    }
}

class Book {
    private String title;
    private String author;

    public Book(String title, String author) {
        this.title = title;
        this.author = author;
    }

    public String getDetails() {
        return title + " by " + author;
    }
}

class Library {
    private List<Book> books = new ArrayList<>();

    public void addBook(String title, String author) {
        books.add(new Book(title, author));
    }

    public void showBooks() {
        System.out.println("Books in Library:");
        for (Book b : books) {
            System.out.println("- " + b.getDetails());
        }
    }
}
```

## OUTPUT:
<img width="1007" height="606" alt="image" src="https://github.com/user-attachments/assets/55ebe6b0-7367-4b43-b0bc-1f66f71114e7" />


## RESULT:

Thus, the Java program demonstrating Composition using Library and Book classes was successfully executed.

