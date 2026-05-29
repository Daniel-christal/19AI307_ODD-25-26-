Ex.No:1(C) LOOPING STATEMENT

QUESTION:
Write a Java program to calculate the factorial of a number using a for loop. The factorial of n is the product of all positive integers less than or equal to n.

<img width="332" height="156" alt="image" src="https://github.com/user-attachments/assets/705b9b7c-5c72-4fba-a7aa-4bcef95b30c1" />

AIM:
To write a Java program that calculates the factorial of a given number using a for loop.

ALGORITHM :
Start the program and read an integer n from the user.

Initialize a variable factorial to 1 to store the result.

Use a for loop from 1 to n, multiplying factorial by the loop counter in each iteration.

After the loop ends, print the value of factorial as the factorial of n.

Stop the program.

PROGRAM:
```
Program to implement a Looping Statement using Java
Developed by: DANIEL C
RegisterNumber: 212223240023

SOURCE CODE:
import java.util.Scanner;

public class FactorialCalculator {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();  
        long factorial = 1;

        for (int i = 1; i <= n; i++) {
            factorial *= i;
        }

        System.out.println("Factorial of " + n + " is: " + factorial);
    }
}
```
OUTPUT:
<img width="861" height="311" alt="image" src="https://github.com/user-attachments/assets/bad86c90-9ece-4a6a-9ffb-ddea4ee6706e" />

RESULT:
The program successfully computes and displays the factorial value of the entered number.
