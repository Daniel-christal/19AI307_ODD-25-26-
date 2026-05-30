# Ex.No:5(D) THREAD PRIORITY

## QUESTION:
Create a program that reads a thread name and a priority (1–10), sets that priority to a new thread, prints both values.

 Input:

Two lines: <threadName>, <priority>

 Output:

Thread <threadName> priority set to <priority>

For example:

Input	Result
Alpha
5
Thread Alpha priority is 5


## AIM:
To develop a Java program to create a thread, set its priority, and display the thread name and priority.

## ALGORITHM :
1.Start the program.

2.Read the thread name and priority from the user.

3.Create a thread with the given name and priority.

4.Start the thread.

5.Display the thread name and its priority.

6.End the program.

## PROGRAM:
 ```

Program to implement a Thread Priority Concept using Java
Developed by: DANIEL C
RegisterNumber:  212223240023

import java.util.Scanner;

class MyThread extends Thread {
    MyThread(String name, int priority) {
        super(name);
        setPriority(priority);
    }

    public void run() {
        System.out.println("Thread " + getName() + " priority is " + getPriority());
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String threadName = sc.nextLine();
        int priority = sc.nextInt();

        MyThread t = new MyThread(threadName, priority);
        t.start();

        sc.close();
    }
}

```



## OUTPUT:

<img width="931" height="397" alt="image" src="https://github.com/user-attachments/assets/79146ed7-7f06-4b4e-adda-11e3d3b2e483" />


## RESULT:
The program successfully creates a thread with the specified priority and displays its name and priority.
