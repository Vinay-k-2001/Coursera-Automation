**Identify Courses**
*******************

**Problem Statement :** Identify Courses
Search and display all web development courses 
1. Should be for beginners level.
2. Courses offered in English language
3. Display first two courses with name, total learning hours and rating.
(Suggested Site: coursera.org however  you are free to choose any other legitimate  site)

**Detailed Description:**
***********************************
1. Search for web development courses for Beginners level & English Language and extract the course names, total learning hours & rating for first 2 courses
2. Look for Language Learning; Extract all the languages and different levels with its total count & display them
3. In Home page, go to "For Enterprise"; Look into Courses for Campus under Product; Fill the  "Ready to transform" form with any one input invalid (example: email); Capture the error message & display
(Suggested Site: coursera.org however  you are free to choose any other legitimate  site)

**Key Automation Scope**
********************
Handling different browser windows, search option
Extract multiple list items & store in collections
Navigating back to home page
Filling form (in different objects in web page)
Scrolling down in web page

**Application URL - https://www.coursera.org/ **

***Test Scenarios and Test Cases For the above Requirement are***
---
Feature: Identify Courses

  Scenario: Search for Web Development Courses
    Given Navigate to the coursera home page
    When the user clicks on the inputBox
    And the user selects the checkBox
    Then verify the name of the first course
    Then verify the rating of the first course
    Then verify the duration of the first course
    Then verify the name of the second course
    Then verify the rating of the second course
    Then verify the duration of the second course

  Scenario: Display the languages and levels
    Given navigate to the learning page
    Then get the languages and their count
    And get the levels and their count

  Scenario: Fill the form
    Given navigate to the Coursera home page
    When the user clicks on For Enterprises
    Then enter the invalid details of email in the form
    And verify the first invalid error message
    Then enter the invalid details of phone in the form
    And verify the second invalid error message
    Then enter the valid details in the form
    And verify the third valid message



**Utility Classes**
***************
1. ExcelUtility.java  - For Writing the data into the Excel sheet and reading data from Excel sheet.

**TestData**
***************
1. ExcelData.xlsx - For retrieving data from Excel sheet to the WebPage and writing data from WebPage to Excel sheet.



**Technologies Used**
*****************
1. Java Programming Language
2. Selenium Automation Tool
3. Cucumber Framework
4. Hybrid Framework
5. Apache Log4j
6. Apache POI
7. AventStack
8. JUnit

**Libraries and Dependencies Used**
*******************************
**selenium-java**   - 4.19.1

**WebDriverManager** - 5.7.0

**apache-poi**      - 5.2.5
**apache-poi-ooxml** - 5.2.5

**testng** - 7.9.0

**cucumber-junit** - 7.15.0
**cucumber-java**  - 7.15.0

**junit** - 4.13.2

**extentreports-cucumber7-adapter** - 1.14.0





