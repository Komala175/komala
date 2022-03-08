# komala
OTP GENERATION IN JAVA
import java.util.*;
public class Otp {
	    public static void main(String[] args)
	    {
	       	        int length = 10;
	        System.out.println(geek_Password(length));
	    }
	  	    static char[] geek_Password(int len)
	    {
	        System.out.println("Generating password using random() : ");
	        System.out.print("Your new password is : ");
	  	        String Capital_chars = "KOMALA";
	        String Small_chars = "devi";
	        String numbers = "9361556005";
	                String symbols = "!@#$5&*";
	  
	  
	        String values = Capital_chars + Small_chars +
	                        numbers + symbols;
	        Random rndm_method = new Random();
	        char[] password = new char[len];	  
	        for (int i = 0; i < len; i++)
	        {
	            
	            password[i] =values.charAt(rndm_method.nextInt(values.length()));
	  
	        }
	        return password;
	    }
	}
