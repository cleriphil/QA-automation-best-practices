# QA Automation Best Practices

## Best Practices in Coding:

- ### Write clear and helpful validation statements. 
   Each assertion method in Testcafe has an optional “message” parameter. The message displays in the report if the test fails. The message must be helpful and clear so that anyone analyzing the report can easily understand the results. 

- ### Validation statements should be clear, helpful messages.
   Testcafe Assertion API - https://devexpress.github.io/testcafe/documentation/test-api/assertions/assertion-api.html

- ### DRY
   Don't Repeat Yourself

- ### Use selectors that are specific and unlikely to change.
   Selectors should use IDs and class names whenever possible. 
    After tests are executed, the test environment may need to be cleaned up.
   If the test permanently alters the site’s settings or content, the site should be restored to its original state. 
 
- ### Name your tests wisely. Make tests more simple instead of adding comments.
- ### All tests should be independent of each other.
  
 - ### Establish naming conventions for files, selectors, etc. 
   Example for selenium: http://makeseleniumeasy.com/2018/07/29/best-practises-in-page-object-model-naming-conventions-of-web-elements-actions-on-it/

- ###  Use the Triple A (AAA) pattern
  > Arrange — In this phase, we set up the testing objects (including Page Objects) and prepare the prerequisites for our test
  > Act — In this phase, we perform the actual work of the test, i.e. invoke the method being tested
  > Assert — In this phase, we verify the result, i.e. check whether the expectations were met 
  https://medium.com/ranorex-webtestit/5-tips-to-keep-your-page-objects-maintainable-3686bd539759

- ### Use Page Objects
   Use Page Objects to store element locators.

   In the directory structure, Page Objects are stored in a separate folder than the tests. 

   All element locators are kept in Page Objects. 
   Assertions are used only in Test files. 

   The Page Object Model makes the code more maintainable. It allows us to update element locators without editing test cases. 

   Other benefits:
   Organizes code structure 
   Helps avoid duplicate element locators

  Other Info:
  Despite the name, a page object does not have to handle an entire page.  On a more complex web page, there can be multiple page objects  that each handle a different UI feature  on the same page. 
  We may have common actions that need to be used across multiple test files. To avoid repeating code, we can store those common actions in a Base Page Object. (In our code, it  is in the lib folder.)

  Resources:  
  Test Cafe docs - Page Object Model - https://devexpress.github.io/testcafe/documentation/recipes/extract-reusable-test-code/use-page-model.htm  
  Page Object Model - https://medium.com/tech-tajawal/page-object-model-pom-design-pattern-f9588630800b  
  Using a Base Page Object - http://elementalselenium.com/tips/9-use-a-base-page-object   
