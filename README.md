import java.util.Scanner;
public class Calculator {
	public static void main(String[] args) {
	string [] arab = new string[10]{"10","1","2","3","4","5","6","7","8","9"};
	string [] rome = new string[10]{"X","I","II","III","IV","V","VI","VII","VIII","IX"};
	double num1;
	double num2;
	double ans;
	char op;
	Scanner reader = new Scanner(System.in);
	System.out.print("Введите два числа: ");
	num1 = reader.nextDouble();
	num2 = reader.nextDouble();
	System.out.print("\nВыберите действие (+, -, *, /): ");
	op = reader.next().charAt(0);
	switch(op) {
		case '+': ans = num1 + num2;
			break;
		case '-': ans = num1 - num2;
			break;
		case '*': ans = num1 * num2;
			break;
		case '/': ans = num1 / num2;
			break;
	default:  System.out.printf("Ошибка! Проверьте правильность ввода");
		return;
	}
	System.out.print("\nРезультат получился следующий:\n");
	System.out.printf(num1 + " " + op + " " + num2 + " = " + ans);
	}
}
