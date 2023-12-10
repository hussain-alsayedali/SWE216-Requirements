The guidelines for making a commit are provided below:




1. Only one change per commit.   ✔️

For example if there is 2 requirements that needs to be changed then you must do them in 2 different commits



2. The commit message must have a title and a body ✔️
For example:

Add teacher login feature
	
	This commit will introduce a new api endpoint for teacher registration. The database changes , backend and frontend are included. This feature will allow the user to login to the system.

3. Leave a space between the title and the body .✔️
Same example as above

4. The message must start with a verb✔️
For example : ADD , DELETE , Update, CREATE

5. If the change would cause some issue in different requirement then it must be added in the same commit. ✔️

Add teacher login feature

	#fixes 477

	This commit will introduce a new api endpoint for teacher registration. The database changes , backend and frontend are included. This feature will allow the user to login to the system.

6. The message should maintain a respectful tone. ✔️

7. The character limit is 400, no commit must exceed this limit ✔️


And for these guidelines here a counter example for which you must avoid doing:

1. More than one change per commit ..❌


Implement user login functionality 
Update requirements of teacher registeraiton
Delete requirement #234 because of inconsistency 


2. Commit with title and without a body or  a body only. ❌

Ex1 :

Implement user registration functionality 

Ex2 :

This commit would add functionality to user recording and would allow them to save them and see them later, this requirement include changes to the schema and the backend.


3. Not leaving a space between the title and body . ❌

Add teacher login feature
	This commit will introduce a new api endpoint for teacher registration. The database changes , backend and frontend are included. This feature will allow the user to login to the system.

4. The commit does not starting with a verb. ❌

Teacher login functionality implemented

5. The commits change a requirement which would affect another and it was not written . ❌

Add teacher login feature
		
(THIS MUST BE WRITTEN IF THE CHANGE WOULD AFFECT ANOTHER #fixes 477)

	This commit will introduce a new api endpoint for teacher registration. The database changes , backend and frontend are included. This feature will allow the user to login to the system.



6. The message is not being respectful. ❌

Implement login for the dumb users

Users are dumb and for that reason we should make the login feature easy to use


7. Long commit message exceeding 400 characters. ❌
Certainly! Here's an example of a commit message that exceeds 400 characters:

```
✅ Add user authentication and authorization functionality

Closes #1234

This commit implements the highly requested user authentication and authorization feature. It introduces a multi-layered security framework to ensure secure access to the system. The backend API endpoints have been updated to handle user registration, login, and password reset functionality. Additionally, user roles and permissions have been implemented to control access to specific resources and actions.

On the frontend, a user-friendly login form has been added, with validation and error handling to provide a seamless experience for users. The UI also includes a user management interface for administrators to assign roles and manage permissions.

To enhance security, password hashing and salting algorithms have been implemented, along with proper session management and token-based authentication. This ensures that user credentials are securely stored and transmitted.

The user authentication and authorization feature greatly enhances the overall system security and user experience. It allows registered users to securely access their accounts and perform actions based on their assigned roles and permissions. This implementation aligns with industry best practices and ensures compliance with security standards.

Overall, this commit delivers a robust and comprehensive user authentication and authorization solution, meeting the project's requirements and addressing the needs of users and administrators alike.

Closes #1234
