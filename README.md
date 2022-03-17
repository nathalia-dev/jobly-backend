# jobly-backend

## Project Description 

jobly-backend is the backend part of Jobly: A application that shows jobs oportunities and enable the user to apply for them. Also, it provides information about each company that is offering a job.

## Project Motivation

Jobly was developed as a bootcamp exercise to practice **Node.js**, **React** and **tests** knowledge. 

## Project Functionalities

- The project is divided by 4 aspects: users, companies, jobs and auth (authentication).
- There is only one user's type: the user who wants to find a job opportunity and apply for it. 
- The user can search for companies and see all the jobs that they are offering. Or the user can search directly for a job, based on the job position. 
- Once the user found the desirable job, he/she can apply for it. It's not possible (yet) to undo the apply action. 
- The authentication process uses a user's *token*. It goes throught the *http request* inside the *header*. To keep the user's logged in, the app uses *local storge*.


## Project Tech Specs

- Express
- Node.js
- JavaScript
- PostgreSQL

##### Important Libraries:

- supertest: a test library for HTTP servers.
- bcrypt: It helps to encrypt the user's password before send it to the database.
- jsonwebtoken: It helps to share security information between two parties: a client and a server.
- jsonschema: It helps to do data format validations.

## Usage 🚀

- First, you are gonna need to install Node.js. In case you don't know if you do have it, you can run in your terminal `node -v `.
- Also, you are gonna need NPM. In case you don't know if you do have it, you can run in your terminal `npm -v `.
- After this, in your terminal, execute `git clone` and make sure you're at project's root folder. 
- Now, its time to install the dependencies. Run `npm install`.
- To setup the database , make sure you do have PostgreSQL installed. 
- From your terminal, inside the project's root folder, run `psql < jobly.sql`. It will create your database and also populate it with an initial set of data. 
- To initiate jobly-backend just run `npm start` from your terminal, inside the project's root folder.  

## Tests

- Jest and SuperTest.
- to execute the tests , run `jest -i ` from your terminal. (make sure you're at project's root folder 😄).

## Future Improvements

- Improve the error messages, to let it less technical and more user friendly. 
- Enable the user to undo the apply action.
- Keep track of user's tokens to invalidaded the old ones. 
