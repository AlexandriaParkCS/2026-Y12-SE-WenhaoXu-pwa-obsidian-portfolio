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
		- Allow for 5 attempts if password does not match
		- If 5 attempts reached, lock account for 5 minutes
Output:
- Success Message / Error Message
- Authentication session token
#
**Whiteboard Creation**
The user's whiteboards

Input:
- Name
- Whiteboard settings
	- Size
	- Templates
Process:
- Assigns whiteboard the name the user gave
- Sets the whiteboard to the user's chosen size
- Sets the whiteboard to the user's chosen template
Output:
- Whiteboard is created
- Whiteboard is saved onto the dashboard
