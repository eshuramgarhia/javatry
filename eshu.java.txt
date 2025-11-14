import java.util.Scanner;

public class LoginDemo {
    public static void main(String[] args) {
        
        // predefined username and password
        String validUsername = "admin";
        String validPassword = "12345";

        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter username: ");
        String username = scanner.nextLine();

        System.out.print("Enter password: ");
        String password = scanner.nextLine();

        // check login
        if(username.equals(validUsername) && password.equals(validPassword)) {
            System.out.println("Login successful! Welcome " + username + ".");
        } else {
            System.out.println("Login failed! Incorrect username or password.");
        }

        scanner.close();
    }
}
