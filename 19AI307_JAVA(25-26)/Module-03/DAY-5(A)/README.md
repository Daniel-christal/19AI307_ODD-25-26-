Ex.No:3(E) INNER CLASS

QUESTION:
Write a Java program to create an inner class and access it from the outer class.

AIM:
To demonstrate accessing an inner class from an outer class in Java.

ALGORITHM :
Create an outer class with a private variable.
Define an inner class inside it with a method to access the outer variable.
In main(), create an object of the outer class.
Use it to create an object of the inner class.
Call the inner class method.
PROGRAM:
```
Program to implement a InnerClass using Java
Developed by: DANIEL C
RegisterNumber: 212223240023

SOURCE CODE:
import java.util.Scanner;

class OuterClass {
    String name;

    OuterClass(String name) {
        this.name = name;
    }

    void display() {
        InnerClass inner = new InnerClass();
        inner.showMessage();
    }

    class InnerClass {
        void showMessage() {
            System.out.println("Hello, " + name + "! This message is from the Inner Class.");
        }
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("");
        String input = scanner.next();
        scanner.close();

        OuterClass outer = new OuterClass(input);
        outer.display();
    }
}
```
OUTPUT:
<img width="1139" height="352" alt="image" src="https://github.com/user-attachments/assets/fb881259-d040-4505-a865-935584b08319" />

RESULT:
The program successfully accesses and prints data from the inner class using the outer class.
