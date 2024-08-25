import java.util.Scanner;

public class SandrinoLab1 {
    public static void main(String[] args) {
        
        // Initialize a Scanner object to read the users input from the console
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter number: ");
        
        // Read an integer input from user
        int n = scanner.nextInt();

        // Print the top border of the pattern (*)
        System.out.println(" *");

        // Generate the upper part of the diamond shape
        for (int i = 1; i <= n; i++) {
            // Print the left border of its current row
            System.out.print(" * ");
            
            // Print ascending numbers from 1 to i
            for (int j = 1; j <= i; j++) {
                System.out.print(j);
            }
            
            // Print descending numbers from i-1 to 1
            for (int j = i - 1; j >= 1; j--) {
                System.out.print(j);
            }
            
            // Print the right border and move to the next line
            System.out.println(" * ");
        }

        // Generate the lower part of the diamond shape
        for (int i = n - 1; i >= 1; i--) {
            // Print the left border of the current row
            System.out.print(" * ");
            
            // Print ascending numbers from 1 to i
            for (int j = 1; j <= i; j++) {
                System.out.print(j);
            }
            
            // Print descending numbers from i-1 to 1
            for (int j = i - 1; j >= 1; j--) {
                System.out.print(j);
            }
            
            // Print the right border and move to the next line
            System.out.println(" * ");
        }
        
        // Print the bottom border of the pattern
        System.out.println(" *");
    }
}
