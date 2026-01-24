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


class Student
{
int rollno;

String name;

Void setData(int r, String n)

{
rollno=r;

name n;
}

Void display ()

{

System.out.printin ("Roll no:" + Rollno);

System.out.printin ("name: " + name);

}

public static void main(String[] args) }

Student s1 = new Student ();

s2. SetData (23, "venu");

s1. display();


}

}


#output
![OUTPUT](2a)











# method overloading 2(b)

b) Java program to implement method overloading
(Same method name with different parameters)

Class overloading

{

int add (int a, int b)

{

return a+b;

}

int add (int a, int b, int c).

{

return a+b+c;

}

double add (double a, double b)

{

return a+b;

}public static void main(String[] args) {

overloading obj = new Overloading ();

System.out.println("sum of towo integers: "

+ obj-add) (10,20));

System.out.printin ("sum ofthree integers:"

+ obf. add (20,30, 40));

System.out.println("sum of two double;"
+ obf. double (10.0,5.0));

}


#output
![OUTPUT](2b)















#implementation of constructer2(c)



c) Java program to implement constructor
(Constructor initializes object values)

Class Student

{

String name;

int marke

int age;

Student (String n, int m, int a) {

name = n;

moriks m;

age = a;

}

Void display()

{

System.out.printin ("name: " + name);

System.out.printin ("Marks:" + monks);

System.out.println("Age: " + age);

}
public static void main(String[] args)
{

Student 51= new Student ("Venu", 99, 15);

s1. display();
}

}


#output

![OUTPUT](2c)

#3(a) constructer overloading 

class Student {
    String name;
    int age;
    int marks;
    Student() {
        name = "Not Assigned";
        age = 0;
        marks = 0;
    }
    Student(String n, int a) {
        name = n;
        age = a;
        marks = 0;
    }
    Student(String n, int a, int m) {
        name = n;
        age = a;
        marks = m;
    }
    void display() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("Marks: " + marks);
    }
    public static void main(String[] args) {
        Student s1 = new Student();               
        Student s2 = new Student("Alice", 20);      
        Student s3 = new Student("Bob", 22, 90);   
        s1.display();
        s2.display();
        s3.display();
    }
}
#output
![OUTPUT](3a)



#3(b) binary search 

import java.util.Arrays;

class BinarySearchDemo {
    public static void main(String[] args) {
        int[] arr = {12, 45, 2, 7, 19, 34, 5};
        int key1 = 19;
        int key2 = 20;
        System.out.print("Elements: ");
        for (int x : arr) {
            System.out.print(x + " ");
        }
        System.out.println();
        System.out.println("Element to search: " + key1);
        Arrays.sort(arr);
        System.out.println("After sorting, the array becomes:");
        for (int x : arr) {
            System.out.print(x + " ");
        }
        System.out.println();
        int pos1 = binarySearch(arr, key1);
        if (pos1 != -1) {
            System.out.println("Element " + key1 + " found at position " + pos1);
        } else {
            System.out.println("Element " + key1 + " not found in the list");
        }
        int pos2 = binarySearch(arr, key2);
        if (pos2 != -1) {
            System.out.println("Element " + key2 + " found at position " + pos2);
        } else {
            System.out.println("Element " + key2 + " not found in the list");
        }
    }
    static int binarySearch(int[] arr, int key) {
        int low = 0, high = arr.length - 1;
        while (low <= high) {
            int mid = (low + high) / 2;
            if (arr[mid] == key)
                return mid + 1; // 1-based indexing
            else if (arr[mid] < key)
                low = mid + 1;
            else
                high = mid - 1;
        }
        return -1;
    }
}

#output
![OUTPUT](3b)


#3(c) bubblesort program
class BubbleSort {

 public static void main(String[] args) {
 int[] arr = {34, 12, 45, 7, 19};
        int n = arr.length;

   System.out.println("Number of elements: " + n);
   System.out.print("Elements: ");
        for (int i = 0; i < n; i++) {
            System.out.print(arr[i] + " ");
        }
        System.out.println();

  for (int i = 0; i < n - 1; i++) {
            for (int j = 0; j < n - 1 - i; j++) {
                if (arr[j] > arr[j + 1]) {
                    int temp = arr[j];
                    arr[j] = arr[j + 1];
                    arr[j + 1] = temp;
                }
            }
        }

   System.out.println("Expected Output (Sorted Array):");
      for (int i = 0; i < n; i++) {
            System.out.print(arr[i] + " ");
        }
    }
}


#output
![OUTPUT](3c)
