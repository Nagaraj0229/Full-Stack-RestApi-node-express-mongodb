# Restapi-node-express-mongodb

Crud application with (html,css,ejs,javascript(nodejs),mongodb&express(framework)) 
______________________________________________________________________________________

INTRODUCTION PART
-----------------
 we need to make and deploy our web application first make sure cloud part storing our codes that is nothing but it is a github so we need to sign up using email id into github account then sign in then, do the configuration steps in gitbash interface then crate new repo for our local project then, do the clone the link of our url into the local machine then, start our work . 
1.make new directory crud_app
2.let do (npm init)
3. initialize our package.json file our wish term words
4. install few npm packages for nodejs code purpose 
    [express,morgan,nodemon,ejs,body-parser,dotenv,mongoose,mongodb,axios]
_____________________________________________________________________________________

purposes of above packages simple notes:
-------------------------------------------

* Express is a web framework for Node.js that makes it easy to create web applications.[routing, middleware, and template engines]
* Morgan is a logger for Express that can be used to log requests and responses [file, a database, or a cloud service]
* Nodemon is a tool that automatically restarts your Node.js application when you make changes to the code
*  EJS is a templating engine for Express that can be used to create dynamic HTML pages. It provides a number of features that make it easy to create complex layouts and forms.
*  Body-parser is a middleware for Express that can be used to parse the body of incoming requests. It can be used to parse a variety of data formats, such as JSON, XML, and form data.
*  Dotenv is a module that can be used to load environment variables from a file. This can be helpful for storing sensitive information, such as passwords and API keys.
*  Mongoose is a MongoDB driver for Node.js that makes it easy to interact with MongoDB databases. It provides a number of features that make it easy to query, insert, update, and delete documents in MongoDB.
*  MongoDB is a document-oriented database that is easy to use and scale. It is a good choice for storing data for web applications.
*  Axios is a library for making HTTP requests in JavaScript. It is a good choice for making requests to APIs.

Here are some simple examples of how these technologies can be used:
--------------------------------------------------------------------------

=> You could use Express to create a simple web application that displays a list of users.
=> You could use Morgan to log requests and responses to a file.
=> You could use Nodemon to automatically restart your Node.js application when you make changes to the code.
=> You could use EJS to create a dynamic HTML page that displays the current time.
=> You could use Body-parser to parse the body of an incoming request that contains a user's name and email address
=> You could use Dotenv to load environment variables from a file that contains your database connection string.
=> You could use Mongoose to create a model for a user document in MongoDB.
=> You could use MongoDB to store data about your users, such as their name, email address, and password.
=> You could use Axios to make a request to an API that returns a list of products.
____________________________________________________________________________________________________________________________________________

file stucture for this :
------------------------
 
crud _app 

assets(front end)
      img
      css
          style.css (for stling for this webapp)
      js

server (modules,codes,mongodb connections and so on..)(backend-server side)
      model(for schema validation,process the data, mongodb methods)
              model.js ( for schema validation)
      controller(user request from resourses to server)
      database (for mongodb connection)
              connection.js (for database connection)

      services
            render.js ( for rendering all routes )
      routes (for routing methods)
            router (for all crud functions)
views(for html contents)(front end)
     include(folder)
          _header.ejs(header part of html-template)
          _footer.ejs(footer part of html-template)
          _form.ejs(form part of html-template)
          _show.ejs(show part of html-template)
     index.ejs(path declare to configure _header & _footer)
     index.html(full html code for live server-view)  [after settting the render to ejs delete this fole to this project]


server.js ( main root file for whole project server run)
package.json ( all installed packages & libraries)
package-lock.json (all install packages & libraries file explores & deep details)
.gitignore ( ignore part(like , unwanted to push the folders & files are stord in this file)
.prettirrc (discipiline for this project)
.eslint  ( for all unused var& declarations are run during our application deployment)
config.env (for port security & database string connection)

____________________________________________________________________________________________________________________________________


1. make http server 

* normal get message using normal http request (then set the port variable for server declaration)
* make env for some configurations (the env file must be on root directory)
 
2.modules 

* set the __dirname access ( using inbuilt path method)
* explain about morgan package and how to use this (this for log informations like ms,ip iaddress,url etc..)

[before start third opeartion learning about ejs(embedded javascript for html templating language)

3.views

* set our (_header,_footer.ejs files & path (index.ejs file) & index.html (for full code)

4. Main section

* set the html elements and tags into the index.html file like (icons,css links,rows,etc...& table format)

5. styling HTML 

* adding the styles code into the individual css file therefore only handles styles

6.tables & forms

* fixed main page all details with all needed user basic details..

7.styling form

*create a design & styles for our user interface form 

8. ejs workflow

*make ejs files (show,upate,add users with html contents) 

here the client part is over so, we delete html files in our project.
then do the server side opearation with routes part (using only exoresss framework)

9. Routes

* set the get, add_user & update_user routes using router with rendering files onto the (services& routes folder)

10. mongodb(database workflow)

* connected to the mongodb database with the userdetails database name [ connected  successfullly ! ?? but , we faced some issues on that like,
 nodemon carsh because we declared undefines or unwanted indexes like use find & use create so disable it on database
 connection.js file so disable or remove that..]

11.Api workflow

* set the all models like schema validation, then do the controller for our crud opearations

12. create (method)

* method for creating function for all declaration functions
* craete some data into database with new unrecoded-uril

13. find & update method

* do the get & put methods using postman to mongodb database

14. delete method

* do the delete method using postman from mongodb collection

15. get single user

* before the get single user operation we create some documents into the mongodb collection 

* then, set the id params into the postman get portal after the enter we get particular data from the collection

16. Using api

* to check the via localhost url via direct access to the server without postman tool

* To find our all data should be shown in our  web application server

17. Create New user 

* insert the new data into the collection using web application server

18. Update New user

* update the new value into the particular document value using web application server

19. Delete the User

* before the delete we create teh new user into teh collections for our easy accessing teh, delete the new user using delete 
  toggle in our web application server


20. Run our web application

* using npm run start command in cli using nodemon method tehn do the add,update & delete the user in web application using ejs rendering 

* finally we make a simple web application

----------------------              heyyyy  !!!!!   -----------------------------



























Creating a CRUD Application with Node.js, Express, MongoDB, HTML, CSS, and EJS


Introduction

In this guide, we will develop and deploy a web application using Node.js, Express framework, MongoDB, HTML, CSS, and EJS templating engine. We'll start by setting up our project on GitHub, configuring the environment, and installing necessary npm packages.

Prerequisites

GitHub account for code hosting
Gitbash for configuration
Node.js and npm installed
Basic understanding of Node.js, Express, MongoDB, HTML, CSS, and EJS

Project Setup

Create a new directory named crud_app.
Run npm init to initialize package.json with your preferred settings.
Install required npm packages using:
css
Copy code
npm install express morgan nodemon ejs body-parser dotenv mongoose mongodb axios
Package Purposes
Express: Web framework for Node.js to build web applications.
Morgan: Logging middleware for Express.
Nodemon: Tool to automatically restart Node.js apps on code changes.
EJS: Templating engine for dynamic HTML.
Body-parser: Middleware for parsing incoming request bodies.
Dotenv: Loading environment variables from a file.
Mongoose: MongoDB driver for Node.js.
MongoDB: Document-oriented database.
Axios: Library for making HTTP requests.
Project Structure
lua
Copy code
crud_app
├── assets
│   ├── img
│   ├── css
│   │   └── style.css
│   └── js
├── server
│   ├── model
│   │   └── model.js
│   ├── controller
│   ├── database
│   │   └── connection.js
│   ├── services
│   │   └── render.js
│   └── routes
│       └── router.js
├── views
│   ├── include
│   │   ├── _header.ejs
│   │   ├── _footer.ejs
│   │   ├── _form.ejs
│   │   └── _show.ejs
│   ├── index.ejs
│   └── index.html
├── server.js
├── package.json
├── package-lock.json
├── .gitignore
├── .prettierrc
├── .eslint
└── config.env
Building the Application
Set up an HTTP server and define the port using environment variables.
Use __dirname to access file paths.
Explain the usage of morgan for request logging.
Views and Templating
Set up EJS views with _header and _footer includes.
Create an index.ejs file to structure the page.
Style the HTML elements in index.html.
Forms and Tables
Design the main page with user details display.
Style the user interface form.
EJS Workflow
Create EJS files for showing, updating, and adding users.
Routing and CRUD Operations
Set up routes with express.Router().
Implement GET, POST, and PUT methods for users.
MongoDB Integration
Connect to MongoDB using Mongoose.
Define models with schema validation.
API Workflow
Create controllers for CRUD operations.
Implement create, find, update, and delete methods.
Testing APIs
Use Postman to test GET, POST, PUT, and DELETE requests.
Test getting a single user with an ID parameter.
Integrating APIs
Access localhost URLs directly to check data retrieval.
Display retrieved data on the web application.
Adding New Users
Add new users through the web application.
Updating Users
Update user information using the web application.
Deleting Users
Delete users using the web application.
Running the Web Application
Use npm run start to run the application with Nodemon.
Test adding, updating, and deleting users through the web interface.
Congratulations, you've successfully created a CRUD web application using Node.js, Express, MongoDB, HTML, CSS, and EJS templating!
























