# Test-Class-4
/**
 * 
 */
package com.yourlogo.pages;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.remote.RemoteWebDriver;

/**
 * @author Gomotse
 *
 *
 * This class will store all the locators and methods of login page
 * 
 */
public class TestClass4 {
	
	RemoteWebDriver driver;
	
 By email=By.id("email");
 By password=By.name("passwd");
 By loginButton=By.name("Sign in");
 

 public TestClass4(RemoteWebDriver driver)
 {
	 this.driver=driver;
	 
 }
 
 public void typeUserName(String uid)
 {
	 driver.findElement(email).sendKeys(uid);
 }
	
 public void typePassword(String pass)
 {
	 driver.findElement(password).sendKeys(pass);
 }
 
 public void clickOnLoginButton()
	 {
		 driver.findElement(loginButton).click();
		 
 }
 }
