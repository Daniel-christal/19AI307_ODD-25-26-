Ex.No:1(E) STRINGS AND MATH FUNCTION

QUESTION:
Write a Java program to reverse a given string.

<img width="396" height="142" alt="image" src="https://github.com/user-attachments/assets/55327640-7edc-4d7d-99f5-1781683c7794" />

AIM:
To write a Java program that reverses a given string entered by the user.

ALGORITHM :
Start the program and read a string input from the user.

Create a StringBuilder object with the input string.

Use the reverse() method of StringBuilder to reverse the string.

Convert the reversed StringBuilder back to a string.

Display the reversed string and stop the program.

PROGRAM:
```
Program to implement a Strings and Math Function using Java
Developed by: DANIEL C
RegisterNumber: 212223240023

SOURCE CODE:
import java.util.Scanner;

public class ReverseString {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String str = scanner.nextLine();
        String reversed = new StringBuilder(str).reverse().toString();
        System.out.println("Reversed string: " + reversed);
        scanner.close();
    }
}
```

OUTPUT:
<img width="865" height="300" alt="image" src="https://github.com/user-attachments/assets/fd64d7cc-7be1-41a0-961e-5352af1e03b3" />

RESULT:
The program successfully displays the reversed version of the input string.
