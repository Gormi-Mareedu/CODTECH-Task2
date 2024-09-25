# CODTECH-Task1
import java.util.Scanner;

public class BasicCalculator {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Input first number
        System.out.println("Enter the first number: ");
        double num1 = sc.nextDouble();

        // Input second number
        System.out.println("Enter the second number: ");
        double num2 = sc.nextDouble();

        System.out.println("Choose the operation (+, -, *, /): ");
        char operator = sc.next().charAt(0);

        double result = 0;
        boolean validOperation = true;

        switch (operator) {
            case '+':
                result = num1 + num2;
                break;
            case '-':
                result = num1 - num2;
                break;
            case '*':
                result = num1 * num2;
                break;
            case '/':
                if (num2 != 0) {
                    result = num1 / num2;
                } else {
                    System.out.println("Error: Division by zero is not allowed.");
                    validOperation = false;
                }
                break;
            default:
                System.out.println("Error: Invalid operation.");
                validOperation = false;
        }

        if (validOperation) {
            System.out.println("The result is: " + result);
        }

        sc.close();
    }
}
