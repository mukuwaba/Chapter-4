import java.util.Scanner;

//This is a sample using the WHILE loop
public class ClassAverage {
    public static void main(String[] args) { // shortcut --> m + TAB

        Scanner input = new Scanner(System.in); //Create a Scanner Object to collect user input

        //Init's
        int total= 0;
        int gradeCounter = 1;

        //Loop through and process the grades
        while(gradeCounter <= 10) { //Loop counter compared to another value
            //while stay true as long as the value of less than or equal to 10
            //allows the while loop to end
            System.out.print("Enter grade: "); //will get the next grade that the user types on
            int grade = input.nextInt();
            total = total + grade; //keeps adding the grades to the running total
            gradeCounter = gradeCounter + 1;
            //can do gradeCounter++
        }
        int average = total / 10;

        System.out.printf("%nTotal of all 10 grades is %d%n", total);// souf + TAB
        System.out.printf("Class average is %d%n," , average);
    }// END: main
}//END: class classAverage
