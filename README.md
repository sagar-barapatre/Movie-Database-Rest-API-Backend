# ### [Movie-Database-Rest-API-Backend](https://github.com/sagar-barapatre/Movie-Database-Rest-API-Backend)
## 📌 Problem Statement

To build an Rest API server like IMDB, where,
● public users can use the service to search for movies by name, genre and be able to sort and filter the results by votes, genre
● Registered/Authenticated users should be able to add movies, upVote/downVote
movies, set favourite genre and get recommendations based on favourite genre.

### 🌐 Live Project - https://movie-database-rest-api.herokuapp.com

### Front-End - EJS + Bootstrap

### Back-End - Node.js(Express.js) & MongoDB(mongoose)

## Tech Stack

### Front-end

-   The front-end client is built as a simple-page-application using EJS
-   Bootstrap 4 is used for page styling.

### Back-end

-   The back-end server is built with Express.js and Node.js in MVC pattern, which provides completed REST APIs for data interaction.
-   Passport.js is used as an authentication middleware in the sever.
-   JSON Web Token (JWT) is used for signing in user and making authenticated requests.

### Database

-   MongoDB is used as the back-end database, which include different data models/schemas (i.e., User, Post and Comment).
-   Mongoose is used to access the MongoDB for CRUD actions (create, read, update and delete).

## Registration Services

● Register/Signup - API for user registration (username/password should be fine)
● Login API - Registered user should be able to login and use other API's

## Services that can be used by registered users only:
● Add Movies API - A registered user is able to add a movie to the DB. A movie does have a name, genre, release date, up-votes, down-votes and reviews.
● Set favourite genre API - A registered user is able to set their favourite genre.
● Get Movie Detail API - A registered user is able get all the details about a movie (name, genre, release date, up-votes, down-votes and reviews)
● UpVote/DownVote API - A registered user is able to upvote or down-vote a movie.
● Add Review API - A registered user is able to add a review for a movie.

## ⭐ How to get started on local system?

1. Clone the Repo by going to your local Git Client and pushing in the command:
git clone https://github.com/sagar-barapatre/Movie-Database-Rest-API-Backend.git
2. Now, push in the command under `Movie-Database-Rest-API-Backend` directory which will install all the dependencies of the project:
`npm install`
3. Make sure you have  `npm`  Node.js installed in your system. MongoAtlas is used, so no need for local MongoDB setup.
4.  MongoAtlas Setup  [https://www.youtube.com/watch?v=7CqJlxBYj-M&feature=youtu.be&t=293](https://www.youtube.com/watch?v=7CqJlxBYj-M&feature=youtu.be&t=293)  
5. Set up your `.env` file and paste in the URI that you get from following the instructions in the video above. Also set token secret to anything, it is used for jwt authentication.
	```
	PORT=2001
	DB_CONNECTION=**your MongoURI**
	EXPRESS_SESSION_SECRET=**your secret key**
	```
	You need to remember to paste in the and . Do NOT share it publicly, and do NOT include the .env file in commits.

6.  [Only once] Run (from the main directory)  `npm run dev` 

7.  Go to  `https://localhost:2001`  to see the application running.
