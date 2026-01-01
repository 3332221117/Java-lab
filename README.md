# tiltle -primitive data types
public class DefaultValues { 

 static byte b;

 static short s;

 static int i;

 static long l;

 static float f;

 static double d;

 static char c;

 static boolean bool;

 public static void main(String[] args) { 

 System.out.println("Default values of primitive data types:");

 System.out.println("byte: " + b);
 
 System.out.println("short: " + s);

 System.out.println("int: " + i);

 System.out.println("long: " + l);

 System.out.println("float: " + f);

 System.out.println("double: " + d);

 System.out.println("char: " + c);

 System.out.println("boolean: " + bool);

 } 

}
#output







![Output](1a)





Tittle QUADRATIC EQUATION
import java.util.Scanner;

public class QuadraticEquation { 

 public static void main(String[] args) { 

 Scanner sc = new Scanner(System.in);

 System.out.print("Enter coefficient a: ");

 double a = sc.nextDouble();

 System.out.print("Enter coefficient b: ");

 double b = sc.nextDouble();

 System.out.print("Enter coefficient c: ");

 double c = sc.nextDouble();

 double discriminant = b * b - 4 * a * c;

 if (discriminant > 0) { 

 System.out.println("Roots are real and distinct.");

 double root1 = (-b + Math.sqrt(discriminant)) / (2 * a);

 double root2 = (-b - Math.sqrt(discriminant)) / (2 * a);

 System.out.println("Root 1: " + root1);

 System.out.println("Root 2: " + root2);

 } else if (discriminant == 0) { 

 System.out.println("Roots are real and equal.");

 double root = -b / (2 * a);

 System.out.println("Root: " + root);

 } else { 

 System.out.println("Roots are complex and imaginary.");

 double realPart = -b / (2 * a);

 double imaginaryPart = Math.sqrt(-discriminant) / (2 * a);

System.out.println("Root 1: " + realPart + " + " + imaginaryPart + "i");

 System.out.println("Root 2: " + realPart + " - " + imaginaryPart + "i");

 } 

 } 

} 
#output
![OUTPUT](1b)



#Tittle implementation of class mechanism 2(a)


class Student {
    int rollNo;
    String name;
    void setData(int r, String n) {
        rollNo = r;
        name = n;
    }
    void display() {
        System.out.println("Roll No: " + rollNo);
        System.out.println("Name: " + name);
    }
    public static void main(String[] args) {
        Student s1 = new Student();  
        s1.setData(23, "venu");      
        s1.display();           
    }
}

#output
![OUTPUT](2a)











# method overloading 2(b)

b) Java program to implement method overloading
(Same method name with different parameters)

class MethodOverloading {
    int add(int a, int b) {
        return a + b;
   }
    int add(int a, int b, int c) {
        return a + b + c;
    }
    double add(double a, double b) {
        return a + b;
    }
    public static void main(String[] args) {
        MethodOverloading obj = new MethodOverloading();
        System.out.println("Sum of 2 integers: " + obj.add(10, 20));
        System.out.println("Sum of 3 integers: " + obj.add(10, 20, 30));
        System.out.println("Sum of 2 doubles: " + obj.add(5.5, 4.5));
    }
}


#output
![OUTPUT](2b)















#implementation of constructer2(c)



c) Java program to implement constructor
(Constructor initializes object values)

class Employee {
    int marks;
    int age;
    String Name;
    Employee(int m, String n,int a) {
        marks = marks;
        Name= name;
        age= a;
    }
    void display() {
        System.out.println("Employee marks: " + Marks);
        System.out.println("Employee Name: " + Name);
        System.out.println("Employee age: " + age);
    }
    public static void main(String[] args) {
        Employee e1 = new Employee(201, "Suresh",19); 
        e1.display();
    }
}


#output

![OUTPUT](2c)





