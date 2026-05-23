The application interacts with a number of external entities (actors) as shown on the following Context Diagram.
![[Pasted image 20260521130420.png]]
The actors include:
- Student: a person who registers, logs in, and interacts with the application to manage their chores and daily tasks, inputting chores and receiving feedback through the dashboard.
- Authentication Provider: a 3rd-party authentication and authorisation provider such as Google. 
- Database: the application uses an SQL database such as SQLite to store financial information for each user.

***Level 1 Data Flow Diagram***
The following diagram shows the top level structure of the application.
![[Pasted image 20260521130516.png]]
Users must login in order to create, manage, or do anything with their chores. To register / login, users must provide valid credentials such as google credentials. 

The users are then presented with a dashboard once they have logged into the application. Users can manage their chores from the dashboard, and the information will be stored in an SQL file.