# QA Automation Best Practices
## Best Practices in Process:

- ### Don’t run ALL tests on ALL browsers.
  For cross-browser testing, it’s not necessary to run all tests on all browsers. Run all tests on one browser and a smaller suite of tests for basic functionality on the other browsers. 


- ### Take screenshot on failure


- ### Separate failing, low-priority test cases 
  If we expect certain lower-priority tests to fail, they should be executed into a separate test run. Otherwise it is harder to analyze the overall test run. 


- ### If there’s a failure, the suite should automatically rerun. If there’s a double failure, then we investigate it. 


- ### Automation should be treated like software development. 
  Use coding best practices, do code reviews, report/track automation bugs, etc. 


Resources:

Automation best practices [2019] - Uploaded by Ultimate QA - https://www.youtube.com/watch?v=r9K-2OJUmOE 
Top 15 UI Test Automation Best Practices You Should Follow -  https://www.blazemeter.com/blog/top-15-ui-test-automation-best-practices-you-should-follow/  
14 Test Automation Best Practices to Supercharge Testing Efficiency - https://blog.testproject.io/2017/04/16/test-automation-best-practices/


