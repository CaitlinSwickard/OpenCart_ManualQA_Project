# OpenCart Manual Testing Portfolio Project

**Project Overview**

This project aims to showcase manual testing skills and knowledge through a simulated testing engagement on OpenCart, a popular e-commerce platform. The focus is on the frontend user experience, testing functionalities of the OpenCart frontend Account management features.

**Key Objectives**

* Demonstrate proficiency in manual testing techniques and methodologies.
* Simulate a real-world testing project to showcase practical application of testing skills.
* Create a comprehensive portfolio artifact highlighting testing efforts and outcomes.

**Scope**

The scope of this testing project includes verifying the following account management functionalities accessible to customers through the OpenCart frontend:

* **Registration:** Creating a new account with valid credentials, error handling for invalid inputs, and account activation process (if applicable).
* **Login:** Successful login with valid credentials, error handling for invalid credentials or account lockout, and "Remember me" functionality.
* **Logout:** Successful logout and redirection to the appropriate page.
* **Forgot Password:** Password reset process, email delivery, and password reset link functionality.
* **My Account:** Access to the "My Account" page after successful login, correct display of user information.
* **My Account Information:** Updating personal information (e.g., name, email, address), data validation, error handling, and password change functionality.
* **Change Password:** Updating / Changing Password functionality and redirection to the appropriate page.

Exclusions

* Any functionalities not explicitly listed in the scope section of the FRS.
* Third-party integrations or payment gateways.
* Automation testing.

**Reporting and Documentation**

* **Functional Requirements Specification (FRS)** [View FRS Doc here](https://docs.google.com/document/d/1-bVXdfGngcGoLbd5w8WY7ChHjOLvLUIpcG8K-jTL0KY/edit?usp=sharing)

* **Test Plan** [View Test Plan Doc here](https://docs.google.com/document/d/1tdDaltpz96mcIyic4b3YI_JSV86wV3Qm-1oeOhZkZxc/edit?usp=sharing)

* **Test Scenarios / Test Cases** [View Test Scenarios / Test Cases here](https://docs.google.com/spreadsheets/d/1MGkPVpS9cQkcfCtVTOELhGkbUk2wyA7HaObMBJVj48A/edit?usp=sharing)

* **Bug Report:** [View Bug Report here](https://docs.google.com/spreadsheets/d/1MGkPVpS9cQkcfCtVTOELhGkbUk2wyA7HaObMBJVj48A/edit?usp=sharing)



# Project Process

**Environment setup**

To establish a testing environment for the OpenCart project, I downloaded and installed OpenCart and XAMPP onto my local machine. I set up XAMPP, a popular local development environment, to host the OpenCart application. This involved configuring the database (MySQL) and web server (Apache) components of XAMPP to interact with OpenCart. Once the application was successfully deployed to the local server, I conducted initial smoke testing to verify the basic functionality and user interface.

**Testing:**

Once the testing environment was ready, I executed each test case outlined in the test plan. This involved interacting with the OpenCart frontend to perform actions like registering new accounts, logging in, resetting passwords, updating account information, and logging out. I carefully observed the system's behavior, recorded test results, and documented any bugs or issues encountered. By following this structured approach, I ensured comprehensive coverage of the specified test cases.



**Bugs / Bug Report:**

Summary of Test Findings
During testing of the OpenCart account management features, several bugs were identified. Here's a breakdown of the key issues:

Registration:
OC-BUG1A: Confirmation email not sent after successful registration (Critical - User cannot verify account)
OC-BUG2: Application allows registration with invalid email addresses (Major - Security risk)
OC-BUG3: Missing visual indicator for mandatory "Privacy Policy" field (Minor - Usability issue)
OC-BUG4: Password complexity requirements not enforced (Major - Security risk)
Login/Logout:
OC-BUG5: User unexpectedly logged out when using browser back button (Critical - Data loss potential)
OC-BUG6: Automatic session timeout not working after 30 minutes of inactivity (Major - Security concern)
Password Reset:
OC-BUG7: Password reset email not sent despite success message (Critical - User cannot recover account)
OC-BUG8: Unclear error message for invalid email formats (Minor - Usability issue)
Navigation:
OC-BUG9: User logged out with invalid token error when accessing "My Account" via site map (Major - Functionality issue)
OC-BUG10: Same issue as OC-BUG9 for "Account Information" (Major - Functionality issue)
OC-BUG11: Same issue as OC-BUG9 for "Password" (Major - Functionality issue)

These bugs range from critical issues, such as the inability to reset passwords or the risk of unauthorized access due to weak password requirements, to minor usability concerns that can hinder the user experience. 


**Testing Performed:**
Overview of Testing Types Performed

* **Black-box testing** was the primary testing methodology employed in this project. This involved testing the application's external behavior without delving into its internal structure. By interacting with the user interface and observing the system's responses, I was able to identify various issues, including incorrect error messages, unexpected behavior, and security vulnerabilities.

* **Sanity testing** was conducted to verify the basic functionality of the application. This involved testing core features like login, logout, password reset, and account information updates. By ensuring that these fundamental aspects were working correctly, it established a solid foundation for further testing.

* **UI testing** focused on ensuring the clarity and accuracy of error messages and text field placeholders. By verifying the consistency and comprehensibility of these elements, aimed to enhance the user experience and minimize potential user errors.


**Project Summary:**

This project involved a comprehensive manual testing effort focused on the account management features of the OpenCart e-commerce platform. The testing environment was set up using XAMPP to host the OpenCart application locally. A series of test cases were meticulously executed to assess the functionality of registration, login, logout, password reset, and account information management. The testing methodology primarily relied on black-box testing, along with sanity testing and user interface testing to ensure the application's correctness, usability, and security.