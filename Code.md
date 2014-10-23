//arithmetic-operators
//====================

//this is a short code to show basic arithmetic operators using java 

// This is my package name
// but in your netbeans or any IDE you are using
// Maybe will find it differenet in the name "javaapplication4"
package javaapplication4;

// This is import statement 
// import from "util" package 
// then access to "Scanner" class 
// "Scanner" class is a predefined class in java
import java.util.Scanner;

// class "JavaApplication4"
// Also maybe will have your own name in the class
public class JavaApplication4 {

    // main method
    // starting point of execution of the program
    public static void main(String[] args){   
        // Create Scanner Object 
        // to get information from the users
        Scanner input = new Scanner(System.in);
        
        // to read choice
        byte choice;
        // Three variable to get two number from user 
        
        int num1 , num2 , result;
        // using "Do-while" loop 
        
        do{
            // show menu for the users
            menu();
            // user will enter his/her choice 
            // and will get saved in "choice" 
            choice = input.nextByte();
            
            // 
            if(choice == 1){
                
                System.out.println("Enter First Number : ");
                num1 = input.nextInt();
                System.out.println("Enter Second Number : ");
                num2 = input.nextInt();
                
                result = add(num1, num2);
                System.out.println(num1 + " + " + num2 + " = " + result);
                
            }else if(choice == 2){
                
                System.out.println("Enter First Number : ");
                num1 = input.nextInt();
                System.out.println("Enter Second Number : ");
                num2 = input.nextInt();
                
                result = sub(num1, num2);
                System.out.println(num1 + " - " + num2 + " = " + result);
                
            }else if(choice == 3){
                
                System.out.println("Enter First Number : ");
                num1 = input.nextInt();
                System.out.println("Enter Second Number : ");
                num2 = input.nextInt();
                
                result = mult(num1, num2);
                System.out.println(num1 + " * " + num2 + " = " + result);
                
            }else if(choice == 4){
                
                System.out.println("Enter First Number : ");
                num1 = input.nextInt();
                System.out.println("Enter Second Number : ");
                num2 = input.nextInt();
                
                result = div(num1, num2);
                System.out.println(num1 + " / " + num2 + " = " + result);
                
            }else if(choice == 5){
                System.out.println("Thank you for using our system.");
                System.out.println();
            }else{
                System.out.println("Wrong Selection. Try Again");
                System.out.println();
            }
            
        }while(choice != 5);
        
    }
    public static void menu(){
        System.out.println("|---------------------------------------------------------------|");
        System.out.println("|                    Calculation                                |");
        System.out.println("|---------------------------------------------------------------|");
        System.out.println("|   1. Sum .                                                    |");
        System.out.println("|                                                               |");
        System.out.println("|   2. Substraction .                                           |");
        System.out.println("|                                                               |");
        System.out.println("|   3. Multplicaton .                                           |");
        System.out.println("|                                                               |");
        System.out.println("|   4. Divion .                                                 |");
        System.out.println("|                                                               |");
        System.out.println("|   5. Exit .                                                   |");
        System.out.println("|                                                               |");
        System.out.println("|---------------------------------------------------------------|");
        System.out.println();
        System.out.println("Enter Your choice : ");
        System.out.println();
    }
    public static int add(int num1 , int num2){
        return num1 + num2;
    }
    public static int sub(int num1 , int num2){
        return num1 - num2;
    }
    public static int mult(int num1 , int num2){
        return num1 * num2;
    }
    public static int div(int num1 , int num2){
        return num1 / num2;
    }
}
