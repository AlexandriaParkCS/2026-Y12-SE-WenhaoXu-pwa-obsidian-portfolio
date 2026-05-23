
**Test Case ID:** TC-002

**Description:** 
- Verify that the login validation works

**Preconditions:**
- A user with a registered email "test@email.com", password "Test1234&%"

**Steps:**
1. Navigate to the login page
2. Submit with nothing in the form
3. Enter email not in database
4. Enter email in database, no password
5. Enter email in database, incorrect password
6. Enter email in database, correct password
 
**Test Data:** 
- Registered email: test@email.com
- Correct Password: Test1234&%
- Incorrect Password: NewPassword99%

**Expected Result:** 
Steps 2-5 should return errors
Step 6 should login, and direct the user to the homepage