Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

QUESTION:
Write a program to access a static variable using both class name and object.

<img width="480" height="176" alt="image" src="https://github.com/user-attachments/assets/e524a097-4c40-4f39-bbaa-56451246092e" />

AIM:
To write a Java program that demonstrates accessing a static variable using both the class name and an object of the class.

ALGORITHM :
Start the program and declare a static variable num inside the class prog.

In the main() method, read an integer value from the user and assign it to the static variable num.

Access and print the static variable using the class name (prog.num).

Create an object of the class (prog obj = new prog();) and access the static variable using the object (obj.num).

Stop the program after displaying the values.

PROGRAM:
```
Program to implement a Variable scope and Constructor using Java
Developed by: DANIEL C
RegisterNumber: 212223240023

SOURCE CODE:
import java.util.Scanner;

class prog {
    
    static int num;

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        num = sc.nextInt();
        System.out.println("Accessing using class name: " + prog.num);

        prog obj = new prog();
        System.out.println("Accessing using object: " + obj.num);

        sc.close();
    }
}
```
OUTPUT:
<img width="943" height="365" alt="image" src="https://github.com/user-attachments/assets/245f4e95-cec1-4f76-b751-bdd2df120088" />


RESULT:
The program successfully shows that a static variable can be accessed directly via the class name and also through an object, producing the same value.
