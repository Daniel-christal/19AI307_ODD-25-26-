Ex.No:2(B) METHODS

QUESTION:
Write a class with one static method and one non-static method. Call both from the main() method.

When staticMethod() is called, it should print "I am static".

When nonStaticMethod() is called, it should print "I am non-static"


<img width="195" height="176" alt="image" src="https://github.com/user-attachments/assets/e8b92a58-391b-4ee7-9da9-6bd45fdf6010" />

AIM:
To create a Java class with one static method and one non-static method, and demonstrate calling both from the main() method.

ALGORITHM :
Start the program and define a class MyClass.

Create a static method staticMethod() that prints "I am static".

Create a non-static method nonStaticMethod() that prints "I am non-static".

In the main() method, call the static method directly using the class name.

Create an object of MyClass and call the non-static method using this object, then stop the program.

PROGRAM:
```
Program to implement a Methods using Java
Developed by: DANIEL C
RegisterNumber: 212223240023
SOURCE CODE:
public class MyClass {
    public static void staticMethod() {
        System.out.println("I am static");
    }
    public void nonStaticMethod() {
        System.out.println("I am non-static");
    }

    public static void main(String[] args) {
        MyClass.staticMethod();
        MyClass obj = new MyClass();
        obj.nonStaticMethod();
    }
}
```
OUTPUT:
<img width="510" height="205" alt="image" src="https://github.com/user-attachments/assets/a528b979-0292-4d6b-b538-f36143f296dc" />

RESULT:
The program successfully calls the static method to print “I am static” and the non-static method to print “I am non-static”.
