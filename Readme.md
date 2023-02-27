Introduction:

The ConvertLength project is a Java program that converts lengths given in feet and inches to centimeters. Length conversion is a common task in 
many fields, such as engineering, construction, and science. Therefore, having a program that can perform this conversion accurately and quickly 
is essential. The ConvertLength program takes input values in feet and inches, converts them to centimeters, and outputs the result. The program assumes 
that the given lengths are integers.

Methodology:

The ConvertLength program is implemented in Java and follows a simple methodology. The program takes input values in feet and inches and converts 
them to centimeters using the following steps:
1.	The program prompts the user to enter the length in feet and inches.
2.	The program reads the input values and stores them in variables.
3.	The program converts the lengths from feet and inches to centimeters using the conversion factor of 1 foot = 30.48 centimeters and 
      1 inch = 2.54 centimeters.
4.	The program outputs the converted length in centimeters.

The program uses the Scanner class to read input values from the user. The program then calculates the total length in inches 
by converting the length in feet to inches and adding the length in inches. The program then converts the total length in inches to centimeters using 
the conversion factor of 1 inch = 2.54 centimeters. The program finally outputs the converted length in centimeters.

Results:

The ConvertLength program takes input values in feet and inches and converts them to centimeters. The output is the converted length in centimeters. Here 
is an example of the input and output of the program:
Enter the length in feet: 5
Enter the length in inches: 8
The length in centimeters is: 172.72	
In this example, the user entered a length of 5 feet and 8 inches, and the program converted it to 172.72 centimeters.

Conclusion:

The ConvertLength program is a simple Java program that converts lengths given in feet and inches to centimeters. The program follows a straightforward 
methodology and is easy to use. The program assumes that the given lengths are integers. The program can be used in various fields where length 
conversion is required. The program can be modified to handle other units of length, such as meters and kilometers. Overall, this project demonstrates 
the use of Java programming language to implement a simple conversion program.








import java.util.Scanner;

/*Problem Statement: Write a program that takes as input given lengths expresses in feet and inches. The program should 
 * then convert and output the lengths in centimeters. Write your code in main() and save your file as "ConverLength.java".
 * Assume that the given lengths in feet and inches are integers.
 * 
 * Author: Divash Pokharel
 * Date: 02/26/23
*/


public class ConvertLength{
    public static void main(String[] args){
        // Step1: Declare the variables
        int feet;
        int inches;
        float cm;
        int extrainch;
        Scanner input =new Scanner(System.in);

        // Step2 : Prompt the user for the input
        System.out.println("ENter the length in feet ");
        feet= input.nextInt();
        System.out.println("ENter the length in inches ");
        inches=input.nextInt();

        // Step 3 : Calculations
        extrainch= feet * 12;
        inches = inches + extrainch;
        cm =((float)inches * 2.54f);

        // PRint the output
        System.out.println("\n The given length in centimeters is "+ cm + " cm.");




        

    }
}
