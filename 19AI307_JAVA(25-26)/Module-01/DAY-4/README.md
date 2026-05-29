Ex.No:1(D) ARRAYS

QUESTION:
Write a Java Program to Find the Average of Array Elements.

<img width="577" height="325" alt="image" src="https://github.com/user-attachments/assets/b7463653-2fed-4866-897e-89a8b4750581" />

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
RegisterNumber: 21222324023
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
<img width="968" height="571" alt="image" src="https://github.com/user-attachments/assets/ae1fb617-56e4-43dc-a768-935f8e3b59b1" />

RESULT:
The program successfully computes and displays the average value of all the array elements entered by the user.
