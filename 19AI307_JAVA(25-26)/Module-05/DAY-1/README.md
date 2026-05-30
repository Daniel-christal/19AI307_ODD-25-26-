# Ex.No:5(A) INPUTSTREAMREADER 

## QUESTION:
Write a program to demonstrate chaining of streams (BufferedReader on top of InputStreamReader on top of System.in)

Input	Result
Ram
25
--- User Details ---
Name: Ram
Age: 25


## AIM:
To develop a Java program that reads a user's name and age from the keyboard using BufferedReader and displays the entered details on the screen.

## ALGORITHM :
1.	Start the program.
2.	
2.Create a BufferedReader object to read input.

3.Read the user's name.

4.Read the user's age and convert it to an integer.

5.Display the user details (name and age).

6.Handle any input errors if they occur.

7.End the program.

## PROGRAM:
 ```
Program to implement a InputStreamReader using Java
Developed by: DANIEL C
RegisterNumber:  212223240023

import java.io.*;

public class Main {
    public static void main(String[] args) {
        try {
            BufferedReader br = new BufferedReader(
                    new InputStreamReader(System.in)
            );

            String name = br.readLine();
            int age = Integer.parseInt(br.readLine());

            System.out.println("--- User Details ---");
            System.out.println("Name: " + name);
            System.out.println("Age: " + age);

        } catch (IOException e) {
            System.out.println("Error reading input");
        }
    }
}
```


## OUTPUT:

<img width="836" height="564" alt="image" src="https://github.com/user-attachments/assets/b40d9874-5ef8-4c13-81e5-67a10b06abd9" />


## RESULT:
The program successfully reads the user's name and age using BufferedReader and displays the entered details on the screen.
