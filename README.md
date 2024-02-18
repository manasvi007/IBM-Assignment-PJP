# Relationships_java
Class relationships in Java define the special relationships among different kinds of classes.
1) **Dependance (Uses-A)**
   When we create an object of a class inside a method of another class, this relationship is called dependence relationship in Java, or simply Uses-A relationship.
   In other words, when a method of a class uses an object of another class, it is called dependency in java. It is the most obvious and most general relationship in java.

   **JAVA**
   
   I have built 3 different files namely:  Library.java, Book.java, Main.java and corresponding code is given below:


          public class Book {
             private String title;

             public Book(String title) {
              this.title = title;
             }
 
             public String getTitle() {
              return title;
             }
         }

            public class Library{
    private Book[] books; // has-a relationship

    public Library(Book[] books) {
        this.books = books;
    }

    public void displayBooks() {
        System.out.println("Books available in the library:");
        for (Book book : books) {
            System.out.println("- " + book.getTitle());
        }
    }
}



         public class Main {
   
          public static void main(String[] args) {
   
              Book[] libraryBooks = {
              new Book("Java Programming"),
              new Book("Data Structures and Algorithms"),
              new Book("Introduction to JavaScript")
            };

              Library myLibrary = new Library(libraryBooks);
              myLibrary.displayBooks();
          }
       }
![image](https://github.com/manasvi007/Relationships_java/assets/98056259/3911e352-3900-40b7-a98e-d124adb7b526)


    
1) **Association (Has-A)**
4) **Inheritance (Is-A)**
   
