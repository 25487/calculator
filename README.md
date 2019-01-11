# calculator
Hallo mijn naam is Taurese Usman

Dit is de code van mijn simple calculator opdracht in java 2-1

Alleen de javac moet gedaan worden nog (heb ik zelf wel al gedaan)






import java.util.Scanner;

public class calculator {

    public static void main(String[] args) {

        Scanner reader = new Scanner(System.in);
        System.out.print("Voer twee getallen in: ");


        double first = reader.nextDouble();
        double second = reader.nextDouble();

        System.out.print("Voer een reken methode in(+, -, *, /, %): ");
        char operator = reader.next().charAt(0);

        double result;

        switch(operator)
        {
            case '+':
                result = first + second;
                break;

            case '-':
                result = first - second;
                break;

            case '*':
                result = first * second;
                break;

            case '/':
                result = first / second;
                break;

            case '%':
                    result = first % second;
                    break;

            default:
                System.out.printf("Fout! Methode bestaat niet of word niet ondersteund");
                return;
        }

        System.out.printf("%.1f %c %.1f = %.1f", first, operator, second, result);
    }
}
