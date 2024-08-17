# Automation Testing Solution for https://automationintesting.online/

## Overview

This project is an automation solution built to test the booking functionality of the website [Automation in Testing](https://automationintesting.online/). 
The tests are written in Java, using the Selenium WebDriver framework and TestNG for test management. 
The codebase is structured to ensure that the core features are thoroughly tested, including opening the website, booking a room, and confirming the booking.

## Prerequisites

- Java JDK: Ensure Java is installed on your machine. You can download it from [Oracle](https://www.oracle.com/java/technologies/javase-downloads.html).
- Maven: Apache Maven is required to manage dependencies and run tests. You can install Maven from [here](https://maven.apache.org/install.html).
- Browser: Install the browser you plan to use for testing (e.g., Chrome).

## Project Structure

- src/main/java/pages/:
  - HomePage.java: Handles interactions on the home page.
  - BookingPage.java: Manages actions on the booking section.
  - ConfirmationPage.java: Validates booking confirmations.

- src/test/java/testcases/:
  - HomePageTest.java: Contains tests for home page interactions.
  - BookingPageTest.java: Tests related to booking a room.
  - ConfirmationPageTest.java: Tests that confirm the booking was successful.

- config.properties: Configuration file that contains test settings such as the URL, browser type, and wait times.

- testng.xml: TestNG suite configuration file that orchestrates the test execution.

- TestBase.java: Base class for setting up and tearing down WebDriver instances.

## How to Run the Tests, Using an IDE:

    Right-click on testng.xml.
    Select "Run As" -> "TestNG Suite".
	
## Customize Configuration

Edit the config.properties file to update:

    url: URL of the site to be tested.
    browser: The browser to use (e.g., Chrome).
    implicit.wait: Implicit wait time in seconds.
    explicit.wait: Explicit wait time in seconds.