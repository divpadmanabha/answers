#Questions

1.	What other possible scenario would you suggest for given page? Suggest 3-5 with your suggestion.


    To test all the fields with equivalence partitions for the acceptable and unacceptable dataset

    Test for Responsive pages - Browser Testing, Mobile Screen Testing etc

    Non-functional tests: Performance of the page, time to first load, time to calculate the eligibility, Browser cache Load etc
    Test for the Look and Feel of the page, as this is a customer facing page

    Localization Testing if applicable. 
    
    Security - DOM Manipulation Tests to see if it would break the UI.


2.	If this test was part of a much larger test suite, how would you speed it up to test particular flow? 

    Create tags, to run the specific use cases in case of failures.
    Create feature specific - .feature files.
    Have setup and tear down mechanism of data - ( Not applicable in this use case )
    Write Independent Test Cases ( Please note: the test cases given were dependant on each other, and hence din't try to implement them otherwise).
    Use of good coding practices to have good reusability within a feature.
    Parallelization - Intermachine or use of dockers for intra-machine execution.

3.  Which approaches could be used to reduce overall execution time? Describe how they could be implemented into your code base.

    Make the test cases independent of each other, once done, we could run them in parallel.
    Use of fewer locators to prevent intensive DOM navigation.
    Handling wait for page load or object load.
    

4.	Sometimes UI tests can fail unpredictably. For example, the page may not have fully loaded before test automation attempts to click a button on a webpage. How would you improve reliability of these tests without increasing execution time?  

    Retry - Use of custom exception handling can provide a fall back mechanism to instigate a retry in case such failure occurs.

5.	From your experience, what is the focus of UI Automation testing – Integration, Functional or Acceptance testing? Briefly explain why.
    
    UI Testing is a very important part of the testing, as at the end of day that's what the customer sees, having said that I also believe that UI test cases should be minimalistic in nature, enough to get the sense of the page is functioning as expected. I believe most of the heavy lifting should be done by the Unit Tests / Contract / API Tests which can validate the functional/business aspects of a test.
    And, if the application performs "business actions" based on the user input in the UI - such use cases are heavily relying on the browser JS, such use cases qualify for UI automation. 


