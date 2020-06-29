# calculator

// import scanner object
import java.util.*;

public class Calculator {
	
	public static void main(String[] args) {
		// declare variables for inputs and operators
		double num1 = 0;
		double num2 = 0;
		char operator;
		double answer = 0.0;
		
		// scanner assigns user input to previously declared variables
		Scanner scanObject = new Scanner(System.in);
		
		System.out.println("Please enter first number: ");
		num1 = scanObject.nextDouble();
		System.out.println("Please enter second number: ");
		num2 = scanObject.nextDouble();
		System.out.println("What operation? ");
		operator = scanObject.next().charAt(0);
		
		// switch case receives operator and chooses case depending on it 
		switch (operator) {
			case '+': answer = num1 + num2;
				break;
			case '-': answer = num1 - num2;
				break;
			case '*': answer = num1 * num2;
				break;
			case '/': answer = num1 / num2;
				break;
		}
		
		// display answer
		System.out.println(num1 + " " + operator + " " + num2 + " = " + answer);
	}
}
