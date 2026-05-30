# Ex.No:5(E) MULTITHREADING -SYNCHRONIZATION

## QUESTION:

Maintain two int variables a and b, read their initial values from user. Use synchronized block to swap them and print swapped values.

Input:

Two lines: a and b values

Output:

a = <swapped_a>

b = <swapped_b>

For example:

Input	Result
5
10
a = 10
b = 5

## AIM:
To develop a Java program to swap two numbers using a synchronized method block and display the swapped values.

## ALGORITHM :
1.Start the program.

2.Read two integers from the user.

3.Create an object with the given values.

4.Swap the values inside a synchronized block.

5.Display the swapped values.

6.End the program.





## PROGRAM:
 ```

Program to implement a Synchronization concept using Java
Developed by: DANIEL C
RegisterNumber:  212223240023

import java.util.*;

class SwapTask {
    int a, b;

    SwapTask(int a, int b) {
        this.a = a;
        this.b = b;
    }

    public void swapAndPrint() {
        synchronized (this) {
            int temp = a;
            a = b;
            b = temp;
        }

        System.out.println("a = " + a);
        System.out.println("b = " + b);
    }
}

public class Main {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();

        SwapTask obj = new SwapTask(a, b);

        obj.swapAndPrint();
    }
}

```



## OUTPUT:

<img width="617" height="395" alt="image" src="https://github.com/user-attachments/assets/59b786c5-b478-4eb8-879d-f559e79d20f6" />


## RESULT:
The program successfully swaps the two numbers using synchronization and displays the swapped values.
