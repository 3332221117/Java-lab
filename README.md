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






