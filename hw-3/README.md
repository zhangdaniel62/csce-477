# Juice Shop Login Form (Security Assignment)

## Overview

This project is a simple login form built using HTML and JavaScript to mimic the login functionality of OWASP Juice Shop. The goal of this project is to demonstrate basic client-side validation and highlight common web security considerations.

## Features

- Email and password input fields
- Client-side validation using JavaScript
- Email validation using regular expressions
- Password complexity enforcement:
  - Minimum 8 characters
  - At least one uppercase letter
  - At least one lowercase letter
  - At least one number
  - At least one special character

## Implementation Details

The email is validated using a regex pattern to ensure proper formatting, and the password is checked against a regex to enforce complexity requirements.

If validation fails, the form prevents submission and displays an alert message to the user.

## Security Considerations

This implementation uses **client-side validation only**, which improves user experience but does not provide real security. Client-side checks can be bypassed using browser developer tools or by disabling JavaScript.

Additionally, the use of `innerHTML` to display user input can introduce potential Cross-Site Scripting (XSS) vulnerabilities if input is not properly sanitized.