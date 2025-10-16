import java.util.Scanner;

public class JavaCaseProblem_JassieferlABaylon {

    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.println("Name: Jassieferl A. Baylon");
        System.out.println("ID Number: 2024303204");
        System.out.println("------------------------------");

        System.out.print("Enter your score (0-100): ");
        int score = input.nextInt();

        String result;
        if (score >= 90 && score <= 100) {
            result = "Excellent! You got an A.";
        } else if (score >= 80) {
            result = "Good job! You got a B.";
        } else if (score >= 70) {
            result = "Fair! You got a C.";
        } else if (score >= 60) {
            result = "Needs Improvement! You got a D.";
        } else if (score >= 0) {
            result = "Sorry, you failed. You got an F.";
        } else {
            result = "Invalid input. Score must be between 0 and 100.";
        }

        System.out.println("------------------------------");
        System.out.println("Result: " + result);

        input.close();
    }
}
