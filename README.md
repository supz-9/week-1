import java.util.Scanner;

public class ReverseNumber {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

       
        System.out.print("Enter a number to reverse: ");
        int number = scanner.nextInt();

        int reversed = 0;
        int original = number;

      
        while (number != 0) {
            int digit = number % 10;         // Extract last digit
            reversed = reversed * 10 + digit; // Append digit to reversed
            number = number / 10;            // Remove last digit
        }

    
        System.out.println("Reversed number of " + original + " is: " + reversed);
    }
}
