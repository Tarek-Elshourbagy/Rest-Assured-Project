# Rest-Assured-Project
## API Automation Assignment
### User API Testing Project
This project is designed to test the various API endpoints of a user management system using RestAssured for API requests and TestNG for organizing and executing the tests. It also uses ExtentReports for generating detailed HTML reports after running the tests.

### Table of Contents
 - Overview
 - Technologies Used
 - Setup Instructions
 - Test Case Descriptions
 - Contributing
### Overview
This project includes test cases for performing CRUD operations (Create, Read, Update, Delete) on user data via a REST API. The tests are built using the TestNG framework, and RestAssured is used to interact with the API.

### Technologies Used
 - Java: Programming language used for writing test scripts.
 - RestAssured: A Java-based library for testing RESTful APIs.
 - TestNG: A testing framework used for running and organizing tests.
 - Maven: Dependency management tool to manage libraries and dependencies.
### Setup Instructions
#### Prerequisites:
 - Java 8 or above installed.
 - Maven installed for dependency management.
 - An IDE like IntelliJ IDEA, Eclipse, or VS Code to run the project.
### Test Case Descriptions
This project includes five test cases that interact with the API as follows:

#### TC_01_Create_User:
 - Description: Creates a new user via a POST request.
 - Verifications: Confirms the response status code is 201, and verifies the name and year fields in the response body.

#### TC_02_List_of_Users:
 - Description: Retrieves a list of users via a GET request.
 - Verifications: Checks the status code 200, ensures the per_page field is 6, the total number of users is 12, and that all users have an avatar URL.

#### TC_03_Search_for_User:
 - Description: Searches for a user by ID via a GET request.
 - Verifications: Ensures the correct user is returned, verifying the name in the response body.

#### TC_04_Update_user:
 - Description: Updates a user's information via a PUT request.
 - Verifications: Verifies that the user’s name and ID are correctly updated in the response body.

#### TC_05_Delete_user:
 - Description: Deletes a user via a DELETE request.
 - Verifications: Verifies that the user is successfully deleted, ensuring the response status code is 204 (No Content).
