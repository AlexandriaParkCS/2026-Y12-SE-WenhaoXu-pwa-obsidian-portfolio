
**Test Case ID:** TC-001

**Description:** 
- Verify that the validation of the Sign Up form works

**Preconditions:**
- The Sign Up form has requirements:
	- Username between 1-50 characters
	- Standard Email requirements
	- Password minimum of 8 characters, one lowercase, one uppercase and one special character
	- AND not repeated

**Steps:**
1. Navigate to the Sign Up page
2. Submit with nothing in the form
3. Enter Case where Username not within requirements
4. Enter Case where Password not within requirements
5. Enter Case where both conditions (Step 3 and 4) hold true
6. Enter Case where repeated username
7. Enter Case where repeated email
 
**Test Data:** 
- Username not within requirements
	- Username: ihaveareallyreallylongnamepleaseletmethrough
- Password not within requirements
	- Password: 1234567
- Both Conditions
	- Username: Z
	- Password: short1
- Repeated Username:
	- Username: testnumone
- Repeated Email: 
	- Email: test@email.com

**Expected Result:** 
Should return errors for all cases.