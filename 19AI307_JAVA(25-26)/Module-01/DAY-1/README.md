Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS
QUESTION:
A shop keeper would like to welcome their customers with their name.

Write a java program to get name from the user (String) and print it.

Input Format:

A single line string input.

Output Format:

Hello, [name]

For example:a

Input : Ajeesh Result : Hello, Ajeesh

AIM:
Write a java program to get name from the user (String) and print it.

ALGORITHM :
1.Start the program.
2.Import the necessary package 'java.util'
3.Create a Scanner object to read input from the user.
4.Read a string input (the user's name).
5.Store the input in the variable name.
6.Display the message: "Hello, " + name
PROGRAM:
/*
Program to implement variables and Operators using Java
Developed by: Daniel C
RegisterNumber:  212223240023
*/
import java.util.*;
public class prog{
    public static void main(String[] args){
        Scanner sc= new Scanner(System.in);
        String name = sc.next();
        
        System.out.print("Hello, "+name);
    }
}
OUTPUT:
Screenshot 2025-11-19 104928
RESULT:
Thus, the java program to get name from the user (String) and print it is executed successfully.
