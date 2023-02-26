import java.util.Scanner;

/*Problem Statement: Write a program that takes as input given lengths expresses in feet and inches. The program should 
 * then convert and output the lengths in centimeters. Write your code in main() and save your file as "ConverLength.java".
 * Assume that the given lengths in feet and inches are integers.
 * 
 * Author: Divash Pokharel
 * Date: 01/25/23
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
