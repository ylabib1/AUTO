package AUTO_Package;

import org.openqa.selenium.WebDriver;
import org.openqa.selenium.firefox.FirefoxDriver;
import org.openqa.selenium.support.ui.Select;
import org.openqa.selenium.*;
import org.openqa.selenium.Keys;



public class AUTO_Class {

	
	 public static void main(String[] args) {
		 
		  WebDriver driver = new FirefoxDriver();
		  
	      driver.get("http://www.goeuro.com/");     
		  driver.findElement(By.id("from_filter")).sendKeys("Berlin, Germany"); 	 
		  driver.findElement(By.id("to_filter")).sendKeys("Prague, Czech Republic");
		  driver.findElement(By.id("search-form__submit-btn")).click();
