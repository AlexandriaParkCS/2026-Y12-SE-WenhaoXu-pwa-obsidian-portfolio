
**Test Case ID:** TC-002

**Description:** 
- Verify account deletion by registering a new account and deleting it.

**Preconditions:**
- None

**Steps:**
1. Navigate to the Sign Up page
2. Create New Account with
		Username: DeleteAccount
		Email: deleteaccount@email.com
		Password: Test1234&%
3. Log into the application
4. Navigate to settings > delete account
5. Enter details and submit
 
**Test Data:** 
- None

**Expected Result:** 
- Account "DeleteAccount" should not appear in the database after deletion.