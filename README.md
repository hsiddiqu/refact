package Date;

import static org.junit.jupiter.api.Assertions.*;

import java.util.ArrayList;
import java.util.List;
import java.util.Scanner;
import java.util.jar.Attributes.Name;




import org.junit.Assert;
import org.junit.jupiter.api.Test;




class renamedTest {

	int Day =1;
	int Month = 1;
	int Year =  2000;
	@Test
	public void Year() {
		 Date date = new Date(Day, Month, Year);
		    Assert.assertTrue(date.getYear() == Year);
		   
		    
		  }
	

	  
	  @Test

	  public void Day() {

	    Date date = new Date(Day, Month, Year);
	    Assert.assertTrue(date.getDay() == Day);
	    
	   
	    
	    
	  }
	  @Test
	  public void DateName(){
		  String testInput = "Date 1\2\2020";
		  Scanner testScanner = new Scanner(testInput);
		  Date notd = new Date(Day);
		    notd.setDate(Day);
		    Assert.assertEquals(23, notd.getDay());
	  }
	  @Test
	   public boolean monthOK(String month)
	    {
	        return (month.equals("January") || month.equals("February") ||
	                month.equals("March") || month.equals("April") ||
	                month.equals("May") || month.equals("June") ||
	                month.equals("July") || month.equals("August") ||
	                month.equals("September") || month.equals("October") ||
	                month.equals("November") || month.equals("December") );
	    }
	  
	   @Test
	    public String monthString(int monthNumber)
	    {
	        switch (monthNumber)
	        {
	        case 1:
	            return "January";
	        case 2:
	            return "February";
	        case 3:
	            return "March";
	        case 4:
	            return "April";
	        case 5:
	            return "May";
	        case 6:
	            return "June";
	        case 7:
	            return "July";
	        case 8:
	            return "August";
	        case 9:
	            return "September";
	        case 10:
	            return "October";
	        case 11:
	            return "November";
	        case 12:
	            return "December";
	        default:
	            System.out.println("Fatal Error");
	            System.exit(0);
	            return "Error"; //to keep the compiler happy
	        }
	    }
	   public void Result() {
		   System.out.println("Display date");
		   
	   }
	 
		 
		 
		  
	  }


	
	


