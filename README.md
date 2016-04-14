# projects

//Assignment 1
//1- Write a method to display a pattern with n lines as follows:
//                1
//              2 1
//            3 2 1
//    .  .  .
//n n-1 ...   3 2 1     
//2- Write a method to display a pattern with n lines as follows:
//                  1
//               2  3
//            4  5  6
//    .  .  .
//       M-2   M-1  M 
//	 [Hint: define a sentinel value.]	   
//The method header is public static void displayPattern2(int n)
package assignment1.sereysathialuy;

import java.util.Scanner;

public class Assignment1SereysathiaLuy {
    public static void main(String[] args) {
        
Scanner input = new Scanner(System.in);

System.out.print("Enter the value of n: ");
int n = input.nextInt();

System.out.println("Project 1:");
System.out.println();
displayPattern(n);

System.out.println("Project 2:");
System.out.println();
displayPattern2(n);

    } //end of main
   
public static void displayPattern(int n) {

for(int i = 1;i<=n;i++){
    
    for(int j=n;j>0;j--){
        
        if(j>i)
            System.out.print("    ");
        else
            System.out.printf("%4d", j);
    }
   System.out.println();
}
    } //end of displayPattern

public static void displayPattern2(int n) {
//M is the sentinel value   
int M = 0;

for (int i = 1; i <= n; i++) {
    
    for (int j = n; j>0; j--) {
        if (j>i)     
        System.out.print("    ");
        else
        System.out.printf("%4d", ++M);
            }
            System.out.println();
        }
    }//end of displayPattern2

} //end of project
