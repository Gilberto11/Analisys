mport java.util.Scanner;

public class Analysis {

  public static void main(String[]args){
  //create a Scanner to obtain input from command window
  Scanner input = new Scanner(System.in);
  //initializing variables in declarations
  int passes =0;//number of passes
  int failures = 0;//number of failures
  int studentCounter = 1;//student counter
  int result;//one exam result(obtain value from user)

  //process 10 students swing counter - controlled loop

  while (studentCounter <=10){
  
  //prompt for the user to input and obtain value from user
  System.out.print("Enter the result(1= pass, 2= fail): ");
  result = input.nextInt();

  //if..else is nested while statement

  if (result ==1) //if result 1
  passes = passes +1;//increment passes

  else //else result is not 1, so
  failures = failures+1; //increment failures

  //increment studentCounter so loop eventually terminates
  studentCounter = studentCounter +1

  }//end whie

  //termination phase, prepare and display results
  System.out.printf("Passed: %d\nFailed: %d\n", passes, failures);

  //determine wheter more than 8 students passed
  if ( passes >8 )
  System.out.println("Bonus to instructor!);

  }//end main

  }//end class Analysis
