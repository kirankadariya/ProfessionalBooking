# ProfessionalBooking
package vacationfinder;

import java.util.Scanner;

public class VacationFinder {

	public static void main(String[] args) {
		
		// Add arrays with vacation destination
		
		String[] sunnyDestinations = {"Bali", "Keys", "Bahamas"};
		String[] snowyDestinations = {"Swiss Alps", "Colorado","Greenland"};
		
		//greet the user
		System.out.println("Welcome to the vacation finder");
		
		//start the scanner
		Scanner scanner = new Scanner(System.in);
		
		//ask the user for a choice
		System.out.println("Do you prefer a sunny vacation");
		
		String response = scanner.next();
		
		//use an if statement to show options
		if(response == "sunny")  {
			System.out.println("Here are some snowy destination you might like!");
			
			
			for( int i=0; i < sunnyDestinations.length; i++) {
				System.out.println("Here are some sunny vacation destinations that you might like to visit:");
			}
			
		} else if (response.equals("snowy")) {
			  System.out.println("Here are some snowy dstination you might like!");
			  
			  
			  for( int i=0; i < snowyDestinations.length; i++) {
					System.out.println("Here are some sunny vacation destinations that you might like to visit:");
				}
				
		}
		else {  
			  System.out.println("Sorry, we only offere ");
		}
		
		//ask user another question
		
		System.out.println("What is the most popular destination");
		System.out.println("Enter A for Swiss Alps, B for Bali, enter C for Colorado");
		
		String ans = scanner.next();
		
		//start a switch
		
		switch(ans) {
		case "A":
		System.out.println("You are correct");
		break;
		case "B":
		System.out.println("You are incorrect");
		break;
		case "C":
		System.out.println("You are incorrect");
		break;
		}

	}

}
