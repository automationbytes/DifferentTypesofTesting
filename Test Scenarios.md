# Facebook Login Page Scenarios and Use Cases

1. **Login with valid username and password.**
   - Verify that the Facebook home page is displayed.

2. **Login with invalid username and password.**
   - Error message stating the username is invalid.

3. **Login with blank username and password.**
   - Error message stating that the username is blank/required.

4. **Login with username and blank password.**
   - Error message stating that the password is blank.

5. **Login with locked user.**
   - Verify that an error message is displayed stating that the user is locked.

6. **Login with case-sensitive user (username with mixed cases).**
   - Verify that the Facebook home page is displayed.

7. **Login with expired password.**
   - Error message stating that the password has expired and needs to be reset.

8. **Login with special characters in username.**
   - Verify that the Facebook home page is displayed or an appropriate error message is shown.

9. **Login with SQL injection attempt in username or password.**
   - Verify that the system handles the input securely and displays an error message.

10. **Login with a very long username or password.**
    - Verify that the system handles the input correctly and displays an appropriate error message if necessary.

11. **Login with a username containing spaces.**
    - Verify that the Facebook home page is displayed or an appropriate error message is shown.

12. **Login with a password containing spaces.**
    - Verify that the Facebook home page is displayed or an appropriate error message is shown.
