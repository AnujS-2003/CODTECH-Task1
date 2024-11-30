**Name:** Anuj Singh Bhadauriya 
**Company:** CODTECH IT SOLUTION 
**ID:** CT08DS9744 
**Domain:** CYBER SECURITY AND ETHICAL HACKING  
**Duration:** October 30th,2024 to November 30th,2024 
**Mentor:** 

**OVERVIEW OF CODE**

This program focuses on secure password validation and authentication. Here's an overview of its functionality:

1. Password Creation
Purpose: Ensure that users create a strong password that complies with security standards.
Process:
Prompts the user to create a password following these rules:
At least 8 characters long.
Contains at least one uppercase letter.
Contains at least one lowercase letter.
Includes at least one digit.
Has at least one special character (e.g., !@#$%^&*()-+).
Validation:
The password is checked against each rule using regular expressions.
If any rule is violated, the program provides detailed feedback, listing all the issues (e.g., "Password must include at least one uppercase letter").
The user can retry until the password meets all criteria.
2. Password Storage
Purpose: Enhance security by avoiding plaintext storage of passwords.
Process:
Once a valid password is entered, it is hashed using the bcrypt library.
The hashed password is stored for future authentication.
Hashing ensures the password itself is not directly saved, making it more secure even if the data is compromised.
3. Password Authentication
Purpose: Allow the user to verify their identity by entering the correct password.
Process:
The user is prompted to enter their password again.
The entered password is compared to the stored hashed password using bcrypt's verification method (checkpw).
Feedback is provided:
Successful Authentication: "Authentication successful!"
Failed Authentication: "Authentication failed. Incorrect password."
4. Security Features
Hidden Input: The password input is hidden from view using the getpass module, preventing anyone nearby from seeing it on the screen.
Limited Attempts: The user gets up to 3 attempts to authenticate. After 3 failed attempts, the program denies access, protecting against brute-force attacks.
Detailed Feedback: During password creation, users receive specific instructions on how to improve their password if it doesn't meet security standards.
Key Highlights
Ease of Use: Provides clear instructions and feedback, making it user-friendly.
Strong Security:
Hashing ensures secure storage of passwords.
Hidden input prevents shoulder-surfing.
Limited attempts add an extra layer of protection.
Modular Design: The program is organized into functions for validation and authentication, making it reusable and easy to extend.
