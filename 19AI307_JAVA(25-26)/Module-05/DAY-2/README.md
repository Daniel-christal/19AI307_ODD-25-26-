# Ex.No:5(B) SERIALIZATION AND DESERIALIZATION 

## QUESTION:

Write a Java program to serialize a collection of objects (like ArrayList<Student>) into a file.

Input	Result
2
101
Alice
89.5
102
Bob
92.0
Students serialized successfully into: students.dat
Students deserialized successfully from: students.dat

Deserialized Students:
Student{id=101, name='Alice', marks=89.5}
Student{id=102, name='Bob', marks=92.0}
## AIM:
To develop a Java program to serialize and deserialize a list of student objects using ObjectOutputStream and ObjectInputStream.

## ALGORITHM :
1.Start the program.

2.Read the number of students and their details.

3.Store the student objects in an ArrayList.

4.Serialize the list and write it to a file.

5.Read the list back from the file using deserialization.

6.Display the deserialized student details.

7.End the program.

## PROGRAM:
 ```
Program to implement a Serialization and Deserialization using Java
Developed by: DANIEL C
RegisterNumber:  212223240023

import java.io.*;
import java.util.*;

class Student implements Serializable {
    int id;
    String name;
    double marks;

    Student(int id, String name, double marks) {
        this.id = id;
        this.name = name;
        this.marks = marks;
    }

    public String toString() {
        return "Student{id=" + id + ", name='" + name + "', marks=" + marks + "}";
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        ArrayList<Student> list = new ArrayList<>();

        for (int i = 0; i < n; i++) {
            int id = sc.nextInt();
            sc.nextLine();
            String name = sc.nextLine();
            double marks = sc.nextDouble();
            list.add(new Student(id, name, marks));
        }

        String fileName = "students.dat";

        // Serialization
        try (ObjectOutputStream out =
                     new ObjectOutputStream(new FileOutputStream(fileName))) {

            out.writeObject(list);
            System.out.println("Students serialized successfully into: " + fileName);

        } catch (Exception e) {
            System.out.println("Error during serialization");
        }

        // Deserialization
        try (ObjectInputStream in =
                     new ObjectInputStream(new FileInputStream(fileName))) {

            @SuppressWarnings("unchecked")
            ArrayList<Student> newList = (ArrayList<Student>) in.readObject();

            System.out.println("Students deserialized successfully from: " + fileName);
            System.out.println();
            System.out.println("Deserialized Students:");

            for (Student s : newList) {
                System.out.println(s);
            }

        } catch (Exception e) {
            System.out.println("Error during deserialization");
        }

        sc.close();
    }
}
```



## OUTPUT:

<img width="1212" height="534" alt="image" src="https://github.com/user-attachments/assets/6d43cc38-8dad-48a7-bfbc-b388bfb9d896" />


## RESULT:
The program successfully serializes the student objects into a file and deserializes them back, displaying the stored student details.
