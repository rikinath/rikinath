import java.time.LocalDate;
import java.time.Period;
import java.time.format.DateTimeFormatter; 
import java.util.Scanner;

public class Log {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Enter your birthdate (yyyy-mm-dd): ");
        String birthdateInput = scanner.next();
        LocalDate birthdate = LocalDate.parse(birthdateInput);

        System.out.println("Enter a date to calculate your age as of (yyyy-mm-dd): ");
        String asOfInput = scanner.next();
        LocalDate asOf = LocalDate.parse(asOfInput);

        Period period = Period.between(birthdate, asOf);
        int years = period.getYears();
        int months = period.getMonths();
        int days = period.getDays();

        System.out.println("You are " + years + " years, " + months + " months, and " + days + " days old as of " + asOf);
    }
}



import java.time.LocalDate;
import java.time.Period;
import java.time.format.DateTimeFormatter; 
import java.util.Scanner;

public class Log {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Enter your birthdate (yyyy-mm-dd): ");
        String birthdateInput = scanner.next();
        LocalDate birthdate = LocalDate.parse(birthdateInput);

        System.out.println("Enter a date to calculate your age as of (yyyy-mm-dd): ");
        String asOfInput = scanner.next();
        LocalDate asOf = LocalDate.parse(asOfInput);

        Period period = Period.between(birthdate, asOf);
        int years = period.getYears();
        int months = period.getMonths();
        int days = period.getDays();

        System.out.println("You are " + years + " years, " + months + " months, and " + days + " days old as of " + asOf);
    }
}
