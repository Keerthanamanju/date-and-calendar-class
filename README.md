# date-and-calendar-class
import java.util.Date;
import java.util.Calendar;
import java.util.Scanner;

public class UserInputDateAndCalendar {
    public static void main(String[] args) {
        
        Calendar calendar = Calendar.getInstance();
        System.out.println("Current Date and Time: " + calendar.getTime());
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of days to add: ");
        int daysToAdd = scanner.nextInt();
        calendar.add(Calendar.DAY_OF_MONTH, daysToAdd);        
        Date updatedDate = calendar.getTime();
        System.out.println("Updated Date: " + updatedDate);
        scanner.close();
    }
}

run:
Current Date and Time: Tue Jan 18 11:30:45 UTC 2022
Enter the number of days to add: 5
Updated Date: Sun Jan 23 11:30:45 UTC 2022

