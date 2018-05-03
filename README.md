package hangman;

import java.util.Random;
import java.util.Scanner;
import java.io.*;


/**
 *
 * @author wooleron
 */
public class HangMan {
    
    private String Movie;
    private int pointsLost;
    private String lettersRight;
    private String lettersWrong;
    private boolean gameOver;
    private String f;
    private String z;
    
    

    public static void main(String[] args) throws IOException{ 
        
    String guess;
        System.out.println ("Lets play a game! a movie title will appear as blanks "
             + "guess the letter in the title name to win!");
        System.out.println (" ");
             
             System.out.println ("Whats the title of the movie shown below?");
    
       
        Scanner scan = new Scanner(new File("List.txt"));
        Scanner name = new Scanner(System.in);
        Random num = new Random();
        int n = num.nextInt(3) +1;
        String out = scan.nextLine();
        args = out.split(",");
        String z = args[n];
        String f = z.replaceAll("[a-zA-Z]","_ ");
        System.out.println (f);
         Scanner kb = new Scanner(System.in);
       guess = kb.next(); 
    
       
    
     
    }
      
     
    }
