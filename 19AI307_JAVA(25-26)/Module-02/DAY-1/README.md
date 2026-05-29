Ex.No:2(A) CLASS AND OBJECT

QUESTION:
Create a class Car with attributes brand, model, year. Create 2 objects and print their details.

<img width="342" height="206" alt="image" src="https://github.com/user-attachments/assets/a9e76778-1d21-4b9f-806f-5f821687e325" />

AIM:
To create a Java class Car with attributes brand, model, and year, and display the details of two car objects.

ALGORITHM :
Start the program and define a class Car with attributes brand, model, and year.

Create a constructor in the Car class to initialize the attributes.

Define a display method in the Car class to print the car details with a label.

In the main method, create two Car objects with different attribute values.

Call the display method for each object to print their details and stop the program.

PROGRAM:
```
Program to implement a Class and Objects using Java
Developed by: DANIEL C
RegisterNumber: 212223240023

SOURCE CODE:
class Car {
    String brand;
    String model;
    int year;

    Car(String brand, String model, int year) {
        this.brand = brand;
        this.model = model;
        this.year = year;
    }

    public void display(String label) {
        System.out.println(label + ": " + brand + " " + model + " " + year);
    }
}

public class CarDemo {
    public static void main(String[] args) {

        Car car1 = new Car("Toyota", "Innova", 2022);
        Car car2 = new Car("Hyundai", "i20", 2021);

        car1.display("Car 1");
        car2.display("Car 2");
    }
}
```
OUTPUT:
<img width="814" height="217" alt="image" src="https://github.com/user-attachments/assets/921d754d-7299-4c68-b4ab-bbef73293db3" />

RESULT:
The program successfully creates two Car objects and prints their brand, model, and year information.
