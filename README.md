# TESTIM-API

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class AutomationTest {
    public static void main(String[] args) {
        System.setProperty("webdriver.chrome.driver", "path/to/chromedriver");

        WebDriver driver = new ChromeDriver();

        driver.get("https://www.orangehrm.com/)");

        driver.findElement(By.id("username")).sendKeys("myusername");
        driver.findElement(By.id("password")).sendKeys("mypassword");
        driver.findElement(By.id("loginBtn")).click();
        
        // Add your automation steps here
        
        driver.quit();
    }
}
