Web Forum Project
Objectives
This project is focused on building a web forum that provides the following functionalities:

User interaction through posts and comments.
Assigning categories to posts.
Liking and disliking posts and comments.
Filtering posts based on various criteria.
Database: SQLite
SQLite is used to manage and store forum data, including users, posts, and comments. As an embedded database, it is widely used for local storage in applications such as web browsers.

To design an efficient database structure and improve performance, it is recommended to create an entity-relationship diagram that aligns with your forum’s data model.

SQL Requirements:
The project must include at least one SELECT, one CREATE, and one INSERT query.
For further details, refer to the SQLite documentation.
Authentication
User authentication is an essential part of this forum, allowing users to register, log in, and participate in discussions.

Registration Requirements:
Users must provide an email address.
If the email is already registered, an error response should be returned.
Users must choose a username.
Users must set a password.
Passwords should be securely stored (encrypting passwords is a bonus task).
Login and Session Management:
Users must log in to post content or leave comments.
Sessions should be managed using cookies, ensuring that each user has only one active session.
Each session must have an expiration date, with the duration configurable by the developer.
Implementing UUIDs for session management is considered a bonus task.
Communication Features
To enable discussion and interaction, users can create posts and comments:

Only registered users can create posts and comments.
Users can assign one or more categories to their posts.
The structure and selection of categories are up to the developer.
All posts and comments are publicly visible, even to non-registered users.
Non-registered users can only view posts and comments but cannot interact with them.
Likes and Dislikes
Only registered users can like or dislike posts and comments.
The number of likes and dislikes on each post and comment should be visible to all users, whether registered or not.
Filtering System
A filtering feature must be implemented to help users find relevant posts. Users should be able to filter posts by:

Categories
Posts they have created
Posts they have liked
Filtering by categories functions as a subforum system, where each category represents a specific discussion topic.

Note: The last two filtering options (created posts and liked posts) are only available for registered users and should be specific to the logged-in user.

Docker Integration
The forum application must be containerized using Docker. For guidance on Docker basics, refer to the ascii-art-web-dockerize documentation.

Development Guidelines
Database: SQLite must be used for data storage.
Error Handling: Proper error handling should be implemented, including HTTP status codes.
Code Quality: The project should adhere to best coding practices.
Testing: It is recommended to include unit test files to validate functionality.
Allowed Packages
Standard Go libraries
sqlite3 for database management
bcrypt for password hashing
UUID for unique identifier generation
Restrictions
Frontend frameworks/libraries such as React, Angular, and Vue are not allowed.
Learning Outcomes
This project provides hands-on experience with:

Web development fundamentals, including HTML and HTTP.
Managing sessions and cookies.
Docker setup and containerization.
Creating and managing database schemas.
Writing SQL queries for data manipulation.
Implementing basic encryption techniques.