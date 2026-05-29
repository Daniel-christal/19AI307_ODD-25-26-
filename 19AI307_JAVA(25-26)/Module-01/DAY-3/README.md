Ex.No:1(C) LOOPING STATEMENT

QUESTION:
Write a Java program to calculate the factorial of a number using a for loop. The factorial of n is the product of all positive integers less than or equal to n.

<img width="334" height="158" alt="image" src="https://github.com/user-attachments/assets/8797aeb4-fb49-4d73-9663-84f16fc36cbf" />

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
Developed by:DANIEL C
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
<img width="887" height="292" alt="image" src="https://github.com/user-attachments/assets/14332532-8a84-4e26-b0ea-75d29a1205fe" />

RESULT:
The program successfully computes and displays the factorial value of the entered number.
