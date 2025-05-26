# BLOG-BACKEND-SYSTEM
*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: Nihar Ranjan Mohapatra

*INTERN ID*: CT04DM1153

*DOMAIN*: BACKEND WEB DEVELOPMENT

*DURATION*: 4 WEEEK

*MENTOR*: NEELA SANTOSH

##  This project is a backend system for a blog platform built with Django and Django REST Framework. It includes all the basic features you’d expect from a blogging site, like user registration and login, creating and managing blog posts, and allowing users to comment on posts. Everything runs on a MySQL database, and the entire system is secured using JWT (JSON Web Token) authentication.

The idea behind this project was to create a solid, secure backend that can easily connect to a frontend—whether that’s a web app, mobile app, or even another service. It’s designed with scalability and clean architecture in mind so it can grow over time with more features.

Main Features
1. User Authentication with JWT
Users can sign up with a username, email, and password, and then log in to receive a secure token. This token is used to access protected parts of the API, like posting a blog or leaving a comment. JWT makes sure that user sessions are stateless and secure, without the need to manage sessions or cookies on the server.

There are three main endpoints for authentication:

Register: Creates a new user.

Login: Returns a JWT token pair (access and refresh).

Token Refresh: Refreshes the access token when it expires.

These are all set up using Django REST Framework’s built-in tools and the simplejwt package.

2. Blog Posts
Once logged in, users can create, view, edit, and delete their blog posts. Each post has a title, content field, author info, and a timestamp for when it was created. Posts are managed through a RESTful API, which means they can be used easily in any frontend or even connected to other platforms.

The /api/posts/ endpoint handles everything related to blog content. All operations (create, read, update, delete) are available for authenticated users, and it’s possible to add more logic later—like making some posts public or private.

3. Comments on Posts
Users can also leave comments on blog posts. Each comment is tied to both a user and a specific post. Just like with blog posts, users can create, edit, and delete their comments using simple API calls.

This feature is great for encouraging interaction and conversation on blog content. It’s also structured in a way that makes it easy to expand—for example, you could add threaded replies or likes in the future.

Database
The backend is powered by a MySQL database, which handles all the data for users, posts, and comments. Django’s ORM takes care of managing tables and relationships between models. You just run a few migration commands, and Django sets up everything for you.

Security
All the key routes—like posting a blog or leaving a comment—are protected, so only logged-in users can access them. JWT is used to manage who is logged in and what they can do. If a token is missing or expired, the API will block the request. This makes it harder for unauthorized users to mess with the data.

Testing with Postman
The entire API is easily testable using Postman. You can register a new user, log in to get your token, and then use that token to test blog and comment features. It’s straightforward to set up, and it helps confirm that everything is working the way it should.

##OUTPUT 


![Image](https://github.com/user-attachments/assets/d32c3395-2184-42f8-84e7-1dd6cbd24006)





##OUTPUT COMMENT IN BLOG

![Image](https://github.com/user-attachments/assets/2bf76b61-beac-48d0-85f6-258bea0bf20e)




