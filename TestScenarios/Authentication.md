# Authentication
## Test Scenarios
Test Scenario ID: TS-001
Title: Verify user registration functionality
Description: Verify that users can create accounts successfully and that duplicate users are handled accordingly.

Test Scenario ID: TS-002
Title: Verify user login functionality
Description: Verify that users can login successfully with valid credentials and invalid login attempts are handled.

### Test Cases
TestCase ID: TC-001
Title: Verify user can create account successfully
Preconditions: Customer must not have an existing account
Steps: 
 1. Navigate to 'Create Account'
 2. Enter valid email address
 3. Enter all required fields
 4. Create valid password
 5. Click 'Sign Up'
Expected Results: Account is created successfully and the user is redirected to the home page
Actual Results: Account is created successfully and the user is redirected to the home page

TestCase ID: TC-002
Title: Verify registration is unsuccessful with existing email address
Preconditions: Email is already exists in the system
Steps: 
 1. Navigate to 'Create Account'
 2. Enter existing email address
 3. Fill in all valid fields
 4. Create password
 5. Click 'Sign Up'
Expected Results: Account registration is unsuccessful and appropriate message is displayed
Actual Results: Account registration is unsuccessfull

