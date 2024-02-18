import java.util.Scanner;

public class MovieDriver {

	public static void main(String[] args){
		Scanner scanner = new Scanner(System.in);
		while (true) {
		Movie movieObject = new Movie();
		System.out.println("Enter the name of the movie");
		String titleInput = scanner.next();
		movieObject.setTitle(titleInput);
		System.out.println("Enter the rating of the movie");
		String ratingInput = scanner.next();
		movieObject.setRating(ratingInput);
		System.out.println("Enter the number of tickets sold for this movie");
		int ticketsInput = scanner.nextInt();
		movieObject.setSoldTickets(ticketsInput);
		System.out.println(movieObject.toString());
		 System.out.println("Do you want to enter another movie? (yes/no)");
         String continueInput = scanner.next();


         if (!continueInput.equalsIgnoreCase("yes")) {
             break; 
         }
     }

     System.out.println("Goodbye");
     scanner.close();
 }}
