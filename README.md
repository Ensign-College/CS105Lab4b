Lab 4b
======

Submit your finished code to the Dropbox. You will need to pass off the lab with the TA or tutor during their office hours (their information is in the CS 105 Course Information section of the Class Resources module), or the instructor in class. Follow the CS 105 Formatting Guide which is also found in the CS 105 Course Information section.

Read the instructions carefully. Make sure your output matches the example run.

Objectives:
===========

In this lab, you will learn how to do the following:

-   Use a do-while loop to perform non-numeric input validation

Structure:
==========

Create the following structure in Eclipse for this lab.

**Package Name:** week4\
**Class Name:** Lab4b

Non-numeric input validation:
=============================

Numbers aren't the only type of data that you may want to validate. Any time you ask the user a question, your program is expecting a certain type of data. For example, you may be asking the user to enter an email address or a password that has specific formatting requirements.

A typical type of question that we will ask the user in labs in this class is the Yes/No question. Your program will ask the user a question and expect the user to answer with either a Yes or No. Your program should perform input validation on the user response to ensure the data entered was either a 'Y' / 'y' / 'N' / 'n'.  Any of these responses are acceptable user input for a Yes/No question. Anything else is not.

Of course, you could expand your list of valid responses to include many other options such as 'Yes' / 'yes' / 'YES' / 'Si' / 'Yep' / 'Yes Sir' / 'No' / 'no' / 'Nope' / 'No way' / etc., but for all labs in CS 105, 'Y' / 'y' / 'N' / 'n' is sufficient.

The basic structure of Non-numeric input validation is similar to that of numeric input validation. The following changes need to be made:

-   **No need** to use try/catch for non-numberic input validation.  Simply use an if statement to determin if the user input matches one of the possible answers the program is looking for.
-   If the example above, the if statement checks to see if the input is either a "Y" or "N" using

*userInput.equalsIgnoreCase("Y") || userInput.equalsIgnoreCase("N")*

Program: Non-numeric Input Validation
=====================================

Write a program that asks the user the Yes/No question as shown in the example run (Do you like to code in Java? (Y/N) ). Perform input validation to ensure that the user entered either a 'Y', 'y', 'N' or 'n'.  AFTER you have received valid input from the user, display the appropriate response as shown in the example run.

Key Program Requirements:
=========================

-   Use a do-while loop to perform input validation on the user input.
-   Use String.equalsIgnoreCase to allow the user to enter 'Y', 'y', 'N', or 'n'.
-   Keep the activities of getting  the valid input and processing the input completely separate.
-   Submit the following .java file:
    -   Lab4b.java

Example Run:
============

-   *Do you like to code in Java?: I do!*\
    *Error: Please answer with a 'Y' or 'N'.*

    *Do you like to code in Java?: Si*\
    *Error: Please answer with a 'Y' or 'N'.*

    *Do you like to code in Java?: Y*\
    *That's great! I do too!*

-   -------------------Restart-------------------------------
-   *Do you like to code in Java?: nope, I don't*\
    *Error: Please answer with a 'Y' or 'N'.*

    *Do you like to code in Java?: N*\
    *That's ok. There are many other wonderful things in life to learn.*