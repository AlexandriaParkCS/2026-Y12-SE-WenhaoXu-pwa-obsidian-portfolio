The application will store its data in an SQL database with the following structure:
![[Pasted image 20260522101709.png]]
The model supports secure user accounts and chore management.

The User entity represents individuals who register and interact with the application. Each user can create and manage multiple chores, with each chore containing information such as the task name, description, scheduled weekday and optional time settings.

The relationships between the entities ensure data integrity and allow efficient retrieval of user-specific chore data. For example, the system can retrieve all chores associated with a particular user to generate personalised schedules, organise weekly task lists, and track completed responsibilities.