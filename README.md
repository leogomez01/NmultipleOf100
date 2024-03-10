import java.util.Scanner;

public class NmultipleOf100 {
    
    public static void main(String[] args) {
    	//Create a scanner object to read user input
        Scanner scanner = new Scanner(System.in);
        
        // We ask the user to enter an integer
        System.out.println("enter a whole number please:");
        int number = scanner.nextInt(); //reads the number entered by the user
        
        // We check if the number entered is a multiple of 100
        if (isamultipleof100(number)) {
        	//prints via console if the number is integer or not depending on the case
            System.out.println("the number entered if it is a multiple of 100");
        } else {
            System.out.println("\r\n"
            		+ "The number entered is not a multiple of 100");
        }
        
    }
    
    /*
      true if the number is a multiple of 100, false otherwise.
     */
    public static boolean isamultipleof100(int number) {
    	/*
    	 Use the modulo operator (%) to check if the number is divisible by 100
         If the remainder of dividing the number by 100 is 0, then it is a multiple of 100
    	 */
        return number % 100 == 0;
    }
}
