Ex.No:1(D) ARRAYS

QUESTION:
Write a Java Program to Find the Average of Array Elements.

<img width="565" height="326" alt="image" src="https://github.com/user-attachments/assets/46d6321d-0da1-4608-a923-7b48a18699e8" />

AIM:
To write a Java program that calculates the average of elements in an array.

ALGORITHM :
Start the program and read the number of elements n from the user.

Create an array of size n and read n integer elements from the user into the array.

Initialize a variable sum to 0 and add all array elements to sum using a loop.

Calculate the average by dividing sum by n and store it in a double variable.

Display the average value and stop the program.

PROGRAM:
```
Program to implement a Array concept using Java
Developed by: DANIEL C
RegisterNumber: 212223240023

SOURCE CODE:
import java.util.Scanner;

public class AverageArray {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int n = scanner.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = scanner.nextInt();
        }
        scanner.close();
        int sum = 0;
        for (int num : arr) {
            sum += num;
        }
        double average = (double) sum / n;
        System.out.printf("The average of elements is %.2f\n", average);
    }
}
```

OUTPUT:

<img width="966" height="578" alt="image" src="https://github.com/user-attachments/assets/7e0d3cff-e406-4980-987f-ab0e241c446e" />

RESULT:
The program successfully computes and displays the average value of all the array elements entered by the user.
