API Automation for Search Deli (Technical Challenge)
This framework is used for performing the API Automation testing for Search Deli Products using the GET Method and uses cucumber BDD where the scenarios in feature file is in readable format.

Scenario: 
1. The Response should contain the status code
2. Validate the status line
3. Get the search count from the response
4. Print the response headers
5. Validate the fields in SearchCount node
6. Validate the ArticleCount matches the test data 
7. The sum of all searches and verify with Total
8. Validate Article count goes below the Threshold
9. UntraceableProductCount should be zero
Tool Requirements
Tool	Description
Eclipse	Sripting tool for Building the Automation
Maven	Build Tool
JDK	Version 1.8
Libraries	Rest Assured, Cucumber BDD, JUnit
Reporting	Extent Reports
Steps to Execute
Step 1: Install Cucumber Eclipse Plugin:

Goto Eclipse -> Help -> Eclipse Marketplace -> Search for 'Cucumber Eclipse Plugin' -> Click Install
Step 2: Download the project from the GIT Repo

Step 3: Import the Maven project into Eclipse

Menu -> File -> Open Projects from File System -> Choose the import Source and Click Finish
Step 4: Expand the Project on Package Explorer

Step 5: Expand src/test/java -> runner file -> open the TestRunner.java

Step 6: To run the testcases, Right Click on TestRunner.java file -> Run As -> JUnit Test

Step 7: Verfiy the Status on the console and Verfiy the Logs in the log file (logs/mylog.log)

Step 8: Refresh the Project Folder and verify the /target/cucumber.json report file

Step 9: To generate the report, Right Click on the Project -> Run As -> Maven verify

Step 10: Validate all the generated Reports under target/cucumber-html-reports/

Assumptions
The Response should contain all the fields in SearchCount node

ProductCount
SpecialProductCount
RecipeCount
ArticleCount
UntraceableProductCount
Total
Assumed and validated the ArticleCount is "12" (if the value changes, it should be updated in src/test/java/TestData/testdata.java)

Assumed to fail the step if the ArticleCount goes below 10

Assumed to fail the step if the UntraceableProductCount is greater than 0

Author
@Suganya Jaganathan
