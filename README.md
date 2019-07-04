# SampleProject

Technologies Used : 

○ .NET core, Visual Studio 2019, Selenium Webdriver

○ Page Object Model (POM) 

○ Nunit Framework 

○ HTML Extent Reporting 

○ Excel Data Reader 

○ AutoIT 

○ Docker 

Improvements:

I was able to improve the existing project Test Framework. 

⦿ I included the HTML Extent Reporting "test log" code in the Tear Down Scenario, where it logs reporting automatically for each test cases, so that you have to focus only on creating your tests as you normally do. This way it improves the code reuseability and a good practise of programming. 
	
⦿ I prefer to capture screenshot only if a test step fails as the images will consume more memory if captured on every test step. If an assert causes a failure, it will be caught, capture screenshot and reported to Extent Reporting. 

⦿ By utilising Assertions and using NUnit, I managed to extract the Test Context for failed test cases in the HTML reporting, so will have better information to investigate test failures.   
[Click here for Sample Extent Report]({% link TestReports/MarsReports.html %})
  
⦿ I believe Test Data should be in the Test Class. Pages only knows how to set and retrieve data from the web page and also verify certain things, But has no clue what data it needs to enter to the page. Test class knows what data and when it needs to send to the page in order to test something. 

⦿ By moving test logic to test controller and handling each test case using a single test method, tests will be run independent of each other. That will eliminate the risk of failing all the test cases instead of having multiple test cases inside a single method of the page object.   

⦿ Refactoring Methods: 
"SelectElement" class in Selenium provides a convenience method for manipulating selections of options in an HTML select element. I have used this method in DropDown selections and was able to reduce the no of code. 
