**Login / Sign Up System**
#
The login system is an important part of the application as it provides security and allows for the user's works to be maintained. 

Input: 
- Username
- Email
- Password

Process:
- Sanitise Username, Email and Password
- Sign Up
	- Check database for matching username AND email
	- If database does not have a matching username AND email, return valid check
	- Check if password matches requirements
	- If password doesn't match requirements, ask the user to enter a password matching the requirements. 
- Log In
	- Check database for matching username AND email
	- If database has a matching username AND email, return valid check
	- Check if password matches username and email
	- If password matches username and email, return valid check
Output:
- Success Message / Error Message
- Authentication session token
#
**Chore Creation**
The user's chores

Input:
- Name
- Chore description
- Chore time
Process:
- Assigns chore the name the user gave
- Sets chore's time to the user's chosen time
- Sets chore description to the description the user chose
Output:
- Chore is created
- Chore sent to the database with User ID
