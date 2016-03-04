package AUTO_Package;

import org.openqa.selenium.firefox.FirefoxDriver;
import org.openqa.selenium.support.ui.Select;
import org.openqa.selenium.*;



public class AUTO_Class {

	
	 public static void main(String[] args) {
		 
		  WebDriver driver = new FirefoxDriver();
		  
	      driver.get("http://www.goeuro.com/");     
		  driver.findElement(By.id("from_filter")).sendKeys("Berlin, Germany"); 	 
		  driver.findElement(By.id("to_filter")).sendKeys("Prague, Czech Republic");
		  
		  try {
			Thread.sleep(2000);
		} catch (InterruptedException e) {
			// TODO Auto-generated catch block
			e.printStackTrace();
		}
		
  
		  
		 driver.findElement(By.id("search-form__submit-btn")).click();
		 driver.findElement(By.id("search-form__submit-btn")).click();
		 
		  try {
			Thread.sleep(2000);
		} catch (InterruptedException e) {
			// TODO Auto-generated catch block
			e.printStackTrace();
		}
		 
