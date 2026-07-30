import java.util.Scanner;
public class VotingEligibility {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);    
        int votingAge = 18; 
        System.out.print("Enter your age: ");
        int age = scanner.nextInt();
        if (age >= votingAge) {
            System.out.println("You are eligible to vote.");
        } else {
            int yearsLeft = votingAge - age;
            System.out.println("You are not eligible to vote.");
            System.out.println("Years left to become eligible: " + yearsLeft);
        }
        scanner.close();
    }
}
