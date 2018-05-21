# First-Project

import java.util.Scanner;

public class Testscore {

		
		//Program Objective
		/* This Program Calculates the weighted test score average, the weighted assignment average,
		 and the master average (average of the two weighted averages) of six test and assignment scores.  */
		
		//Program Instructions
		/* Once run, the program will ask you for the number of tests you wish to take the average of.
		 * Enter 6).
		 * The Program will ask for each individual test score and weight. Enter the correct values when prompted.
		 * When finished, You will get the weighted test score average and be asked how many assignments you wish to take the average of.
		 * Enter 6.
		 * The Program will ask for each individual assignment score and weight. Enter the correct values when prompted.
		 * When finished, you will get the weighted assignment score average and the master average (overall grade).
		 */
	
		//Program code
		/* The program uses scanner, print, and switch functions. I hope to create a different version of this program that can calculate the
	       weighted average of up to six test scores and six assignment scores. 
		 */


			
		public static void main(String[] args) {
			
			int testnum; // testnum = number of tests taken
			double T1, T2, T3, T4, T5, T6; //T = Test score
			double W1, W2, W3, W4, W5, W6; // W = Weight of test
			double var1, var2, var3, var4, var5, var6; // var = Test Score * Test weight
			double AverageWTS; //averageWTS = Average Weighted Test Score
			
			int assignmentnum; // assignmentnum = number of Assignments graded
			double A1, A2, A3, A4, A5, A6; //A = Assignment score
			double AW1, AW2, AW3, AW4, AW5, AW6; // AW = Assignment weight
			double Avar1, Avar2, Avar3, Avar4, Avar5, Avar6; // Avar = Assignment Score * Assignment weight
			double AverageWAS; // averageWAS = Average Weighted Assignment Score
			double Masteraverage; // Masteraverage = Final grade or average of the two weighted averages (AverageWTS and Average WAS)
			
			System.out.print(" How many tests do you wish to take the average of? ");	
			Scanner scan = new Scanner(System.in);
			testnum = scan.nextInt();
			System.out.println(" You have entered " + testnum);
						
			switch (testnum) {
			
			default: System.out.print("Error, You have entered a value other than 6 ");
			break;
			
			case 6:
				
				System.out.print("Enter the first test score");
				Scanner scan1 = new Scanner(System.in);
				T1 = scan1.nextDouble();
				System.out.print("Enter the Weight for the first test score");
				W1 = scan1.nextDouble();
				System.out.print("Enter the second test score");
				Scanner scan2 = new Scanner(System.in);
				T2 = scan2.nextDouble();
				System.out.print("Enter the Weight for the second test score");
				W2 = scan2.nextDouble();
				System.out.print("Enter the third test score");
				Scanner scan3 = new Scanner(System.in);
				T3 = scan3.nextDouble();
				System.out.print("Enter the Weight for the third test score");
				W3 = scan3.nextDouble();
				System.out.print("Enter the fourth test score");
				Scanner scan4 = new Scanner(System.in);
				T4 = scan4.nextDouble();
				System.out.print("Enter the Weight for the forth test score");
				W4 = scan4.nextDouble();
				System.out.print("Enter the fifth test score");
				Scanner scan5 = new Scanner(System.in);
				T5 = scan5.nextDouble();
				System.out.print("Enter the Weight for the fifth test score");
				W5 = scan5.nextDouble();
				System.out.print("Enter the sixth test score");
				Scanner scan6 = new Scanner(System.in);
				T6 = scan6.nextDouble();
				System.out.print("Enter the Weight for the sixth test score");
				W6 = scan6.nextDouble();
				
				var1 = T1 * W1;
				var2 = T2 * W2;
				var3 = T3 * W3;
				var4 = T4 * W4;
				var5 = T5 * W5;
				var6 = T6 * W6;
				
				AverageWTS = (var1 + var2 + var3 + var4 + var5 + var6);
				System.out.print(" The weighted average of the six test scores is " + AverageWTS);
				
				System.out.print(" How many assignments do you wish to take the average of? ");	
				Scanner scan123 = new Scanner(System.in);
				assignmentnum = scan123.nextInt();
				System.out.println(" You have entered " + assignmentnum);
							
				switch (assignmentnum) {
				
							
					
				case 6:
				
				System.out.print("Enter the first assignment score");
				Scanner scan1A = new Scanner(System.in);
				A1 = scan1A.nextDouble();
				System.out.print("Enter the Weight for the first assignment score");
				AW1 = scan1A.nextDouble();
				System.out.print("Enter the second assignment score");
				Scanner scan2A = new Scanner(System.in);
				A2 = scan2A.nextDouble();
				System.out.print("Enter the Weight for the second assignment score");
				AW2 = scan2A.nextDouble();
				System.out.print("Enter the third assignment score");
				Scanner scan3A = new Scanner(System.in);
				A3 = scan3A.nextDouble();
				System.out.print("Enter the Weight for the third assignment score");
				AW3 = scan3A.nextDouble();
				System.out.print("Enter the fourth assignment score");
				Scanner scan4A = new Scanner(System.in);
				A4 = scan4A.nextDouble();
				System.out.print("Enter the Weight for the forth assignment score");
				AW4 = scan4A.nextDouble();
				System.out.print("Enter the fifth assignment score");
				Scanner scan5A = new Scanner(System.in);
				A5 = scan5A.nextDouble();
				System.out.print("Enter the Weight for the fifth assignment score");
				AW5 = scan5A.nextDouble();
				System.out.print("Enter the sixth assignment score");
				Scanner scan6A = new Scanner(System.in);
				A6 = scan6A.nextDouble();
				System.out.print("Enter the Weight for the sixth assignment score");
				AW6 = scan6A.nextDouble();
				
				Avar1 = A1 * AW1;
				Avar2 = A2 * AW2;
				Avar3 = A3 * AW3;
				Avar4 = A4 * AW4;
				Avar5 = A5 * AW5;
				Avar6 = A6 * AW6;
				
				AverageWAS = (Avar1 + Avar2 + Avar3 + Avar4 + Avar5 + Avar6);
				System.out.print(" The weighted average of the six assignment scores is " + AverageWAS);
				
				Masteraverage = ((AverageWTS + AverageWAS) / 2);
				System.out.print(" The master average is " + Masteraverage);
						
					break;
					
				default:
						System.out.print(" Error, You have entered a value other than 6");
				break;
				
						
				
				}}}}
