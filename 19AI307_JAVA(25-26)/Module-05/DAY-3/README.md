# Ex.No:5(C)  FILE HANDLING USING JAVA
## QUESTION:

Write a Java program to create a new file named example.txt.

For example:

Result
File created: example.txt

## AIM:
To develop a Java program to create a new file using the File class.

## ALGORITHM :
1.	Start the program.
2.	
2.Create a File object for the file name.

3.Use createNewFile() to create the file.

4.Display whether the file was created or already exists.

5.Handle any file creation errors.

6.End the program.

## PROGRAM:
 ```

Program to implement a File Handling using Java
Developed by: DANIEL C
RegisterNumber: 212223240023


import java.io.*;

public class Main {
    public static void main(String[] args) {

        try {
            File file = new File("example.txt");

            if (file.createNewFile()) {
                System.out.print("File created: example.txt");
            } else {
                System.out.print("File already exists: example.txt");
            }

        } catch (IOException e) {
            System.out.print("Error creating file");
        }
    }
}
```








## OUTPUT:
<img width="751" height="247" alt="image" src="https://github.com/user-attachments/assets/08f045a5-ce1c-47ea-b878-20f91c3be46c" />



## RESULT:
The program successfully creates a new file if it does not exist and displays the appropriate message.
