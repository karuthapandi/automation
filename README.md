# automation

package selenium;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.firefox.FirefoxDriver;

public class Testing {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		WebDriver driver=new FirefoxDriver();
		driver.get("https://edit.europe.yahoo.com/registration");
		driver.manage().window().maximize();
		driver.findElement(By.id("first-name")).sendKeys("A");
		driver.findElement(By.id("last-name")).sendKeys("Karuthapandi");
		driver.findElement(By.id("user-name")).sendKeys("a_karuthapandi");
		driver.findElement(By.id("password")).sendKeys("Kpandi@123");
		driver.findElement(By.id("mobile")).sendKeys("9677225101");
		driver.findElement(By.id("male")).click();

		driver.findElement(By.id("mobile-rec")).sendKeys("9629806093");
		driver.findElement(By.id("relationship")).sendKeys("hiii");
		driver.findElement(By.className("button submit btn-purple")).click();

		
		
		
	}

}
