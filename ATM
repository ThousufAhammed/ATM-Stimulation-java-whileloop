import java.util.Scanner;

public class ATM {
    public static void main(String[] args){
        // ATM Simulation
        int balance = 5000;
        int pin = 1234;
        int choice;
        Scanner sc = new Scanner(System.in);
        System.out.println("Welcome to the ATM!");
        System.out.println("Please enter your pin: ");
        int enterpin = sc.nextInt();
        while (true){
            System.out.println("ATM Menu: ");
            System.out.println("1. Check Balance");
            System.out.println("2. Deposite Money");
            System.out.println("3. Withdraw Money");
            System.out.println("4. Exit");
            System.out.println("Please enter your choice: ");
            choice = sc.nextInt();
            if (choice == 1){
                System.out.println("Your current balance is: " + balance);
            } else if (choice == 2) {
                System.out.println("Enter the amount to deposite");
                int deposite = sc.nextInt();
                if (deposite > 0) {
                    balance += deposite;
                    System.out.println("Deposited: " + deposite);
                    System.out.println("New Balance: " + balance);
                }else {
                    System.out.println("Invalid deposit amount. Please try again.");
                }
            } else if (choice == 3) {
                System.out.println("Enter the withdraw amount" + balance);
                int withdraw = sc.nextInt();
                if (withdraw > 0 && withdraw <= balance){
                    balance -= withdraw;
                    System.out.println("withdrawn: " + withdraw);
                    System.out.println("New Balance: " + balance);
                } else if (withdraw > balance) {
                    System.out.println("Insufficient balance. Please try again.");
                } else {
                    System.out.println("Invalid withdraw amount. Please try again.");
                }
            } else if (choice == 4) {
                System.out.println("Thank you for using the ATM. Goodbye!");
                break;
            } else {
                System.out.println("Invalid choice. Please try again.");
            }
            if (enterpin != pin) {
                System.out.println("Incorrect PIN. Please try again.");
                System.out.println("Please enter your pin: ");
                enterpin = sc.nextInt();
            } else {
                System.out.println("PIN accepted.");
            }
            if (enterpin == pin) {
                System.out.println("Welcome to the ATM!");
            } else {
                System.out.println("Incorrect PIN. Exiting...");
                break;
            }
        }
    }
}
