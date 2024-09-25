import java.util.Scanner;

public class StudentGradesManager {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Get the number of subjects or assignments
        System.out.println("Enter the number of subjects/assignments: ");
        int numberOfSubjects = sc.nextInt();

        double[] grades = new double[numberOfSubjects];
        double sum = 0;

        // Input grades for each subject/assignment
        for (int i = 0; i < numberOfSubjects; i++) {
            System.out.println("Enter the grade for subject/assignment " + (i + 1) + ": ");
            grades[i] = sc.nextDouble();
            sum += grades[i];
        }

        double average = sum / numberOfSubjects;

        char letterGrade = getLetterGrade(average);

        System.out.println("Average Grade: " + average);
        System.out.println("Letter Grade: " + letterGrade);
        System.out.println("GPA: " + getGPA(letterGrade));

        sc.close();
    }

    // Method to determine the letter grade based on average
    public static char getLetterGrade(double average) {
        if (average >= 90) {
            return 'A';
        } else if (average >= 80) {
            return 'B';
        } else if (average >= 70) {
            return 'C';
        } else if (average >= 60) {
            return 'D';
        } else {
            return 'F';
        }
    }

    // Method to calculate GPA based on letter grade
    public static double getGPA(char letterGrade) {
        switch (letterGrade) {
            case 'A':
                return 4.0;
            case 'B':
                return 3.0;
            case 'C':
                return 2.0;
            case 'D':
                return 1.0;
            case 'F':
                return 0.0;
            default:
                return 0.0;
        }
    }
}
