Ex.No:4(A) EXCEPTION HANDLING

QUESTION:
You wrote a program that stores some input strings into a String array and prints each string in uppercase. However, you're getting a NullPointerException. What should you check in your array before calling .toUpperCase() on a element?

AIM:
To handle a NullPointerException when performing operations on a null string in Java.

ALGORITHM :
Read a string input from the user.
If the input is "null", assign null to the variable.
Try converting the string to uppercase using toUpperCase().
Catch and handle the NullPointerException if the string is null.
Print "Null element" in case of exception.
PROGRAM:
```
Program to implement a Exception Handling using Java
Developed by: DANIEL C
RegisterNumber: 212223240023

SOURCE CODE:
import java.util.Scanner;

public class NullPointerArrayExample {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String input = sc.next();
        String str = input.equalsIgnoreCase("null") ? null : input;

        try {
            System.out.println(str.toUpperCase());
        } catch (NullPointerException e) {
            System.out.println("Null element");
        }

        sc.close();
    }
}
```
OUTPUT:
<img width="670" height="344" alt="image" src="https://github.com/user-attachments/assets/599008c8-aa3d-458c-8adb-4014984e39b6" />

RESULT:
The program successfully detects and handles NullPointerException by displaying "Null element" when the input is null.
