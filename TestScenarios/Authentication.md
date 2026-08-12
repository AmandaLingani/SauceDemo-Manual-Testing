# Authentication
## Test Scenarios
Test Scenario ID: TS-001
## Title: 
Verify user registration functionality
## Description:
Verify that users can create accounts successfully and that duplicate users are handled accordingly.

Test Scenario ID: TS-002
Title: Verify user login functionality
Description: Verify that users can login successfully with valid credentials and invalid login attempts are handled.

### Test Cases
Test Case ID: TC-001
Title: Verify user can create account successfully
Preconditions: Customer must not have an existing account
Steps: 
 1. Navigate to 'Sign Up'
 2. Enter valid email address
 3. Enter all required fields
 4. Create valid password
 5. Click 'CREATE'
Expected Results: Account is created successfully and the user is redirected to the home page
Actual Results: Account is created successfully and the user is redirected to the home page
Status: PASS

Test Case ID: TC-002
Title: Verify registration is unsuccessful with existing email address
Preconditions: Email already exists in the system
Steps: 
 1. Navigate to 'Sign Up'
 2. Enter existing email address
 3. Fill in all valid fields
 4. Create password
 5. Click 'CREATE'
Expected Results: Account registration is unsuccessful and appropriate message is displayed
Actual Results: Account registration is unsuccessful and validation message is displayed "This email address is already associated with an account. If this account is yours, you can reset your password"
Status: PASS

Test Case ID: TC-003
Title: Verify login is successful with the correct credentials
Preconditions: User account already exists
Steps:
 1. Navigate to 'Login'
 2. Enter valid login credentials
 3. Click 'Sign In'
Expected Results: Login is successful and user is redirected to Home page
Actual Results: Login is successful and user is redirected to Home Page
Status: PASS

Test Case ID:TC-004
Title: Verify login is unsuccessful with empty email field
Preconditions: Customer is registered
Steps:
 1. Navigate to 'Login'
 2. Leave 'Email address' field empty
 3. Enter correct password
 4. Click 'Sign In'
Expected Results: Login is unsuccessful and appropriate error message is displayed
Actual Results: Login is unsuccessful and error message is displayed "Incorrect email or password."
Status: PASS

Test Case ID:TC-005
Title: Verify login is unsuccessful with incorrect password
Preconditions: Customer is registered
Steps:
 1. Navigate to 'Login'
 2. Enter correct email address
 3. Enter incorrect password
 4. Click 'Sign In'
Expected Results: Login fails and appropriate error message is displayed
Actual Results: Login fails and error message is displayed "Incorrect email or password."
Status: PASS

Test Case ID:TC-006
Title: Verify login fails when incorrect email address is entered
Preconditions: Customer is registered
Steps:
 1. Navigate to 'Login'
 2. Enter incorrect email address
 3. Enter correct password
 4. Click 'Sign In'
Expected Results: Login fails and appropriate error message is displayed
Actual Results: Login fails and error message is displayed "Incorrect email or password."
Status: PASS

