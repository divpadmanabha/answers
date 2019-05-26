#Questions

1.	What other possible scenario would you suggest for given page? Suggest 3-5 with your suggestion.


    Scenario 1: To test all the fields with boundary value analysis and equivalence partitions for the acceptable and unacceptable dataset

    Scenario 2:  Non-functional tests: Performance of the page, time to first load, time to calculate the eligibility etc

    Scenario 3: Test for the Look and Feel of the page, as this is a customer facing page

    Scenario 4: Integration test to see how this page works with rest of the website

    Scenario 5: Test for responsive pages- Browser Testing, Mobile Screen Testing etc


2.	If this test was part of a much larger test suite, how would you speed it up to test particular flow? 

    Parallelization- Intermachine or use of dockers for intra-machine execution, Use of API, Use of fewer locators to prevent intensive DOM navigation, Use of good coding practices to avoid delayed executionWhich approaches could be used to reduce overall execution time? Describe how they could be implemented into your code base.

3.	Sometimes UI tests can fail unpredictably. For example, the page may not have fully loaded before test automation attempts to click a button on a webpage. How would you improve reliability of these tests without increasing execution time?  

    Use of API’s for navigational part of the automation test is a good way to improve the reliability without effecting the scope of testing. Use of custom exception handling can provide a fall back mechanism to instigate a page refresh in case such failures occue

4.	From your experience, what is the focus of UI Automation testing – Integration, Functional or Acceptance testing? Briefly explain why.

    It’s all three of them. An Application under test can have several components that are back end in nature, but these always present in a UI format when being delivered to a customer. Having said that, there are several products that are purely backend in the sense that the end customers may consume the product as a service. But for the applications that have a customer UI facing component, all three faces of testing require UI automation, albeit to a varying degree of it

