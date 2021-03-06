## 14 Model-View-Controller (MVC): Tech Blog

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Description

The task of this project is to build a CMS-style blog where users can publish articles, blog posts, thoughts and opinions.  

This application will follow the MVC paradigm in its architectural structure, using Handlebars.js as the templating language, sequelize as the ORM, and the express-session npm package for authenication.

The URL of the GitHub repository is <strong>https://github.com/stellalph/14-MVC-Tech-Blog.git</strong>.
and the repository name is 14-MVC-Tech-Blog.

The URL of the deployed application to Heroku is <strong>https://stark-tor-51492.herokuapp.com/</strong>.

The overview of the deployed application to Heroku :-

![alt text](/assets/img14.png)

## Table of Contents

* [Installation](#installation)
* [Usage](#usage)
* [References](#references)
* [License](#license)

## Installation

* The application follows the Model-View-Controller paradigm.  The Model-View-Controller(MVC) is an architectural pattern that adheres to the separation of concerns principle.

* The folder structure for the application will be set up according to this MVC paradigm.

  - The Model - stores data and data-related logic
  - The View - the UI/UX concerns, or what a user will see and interact with.
  - The Controller - the interface between Models and Views.  It processes requests from the View, uses the Model to manipulate data, and sends data to the View to render.

* This application will need the installation of node.js from the website, https://www.node.org.

* Node Package Manager (npm) is a software manager and installer which puts the modules in place so that the node project can utilize it, and also, it manages dependency conflicts intelligently and initialized using <strong>npm init</strong>.  The package.json will be generated and will contains all the details of the application in which the user have inputted during the npm initialization.

* This application will need the [express-handlebars](https://www.npmjs.com/package/express-handlebars) package to implement Handlebars.js for the Views, use the [MySQL2](https://www.npmjs.com/package/mysql2) and [Sequelize](https://www.npmjs.com/package/sequelize) packages to connect to a MySQL database for the Models, and create an Express.js API for the Controllers.

* This application will also need the [dotenv package](https://www.npmjs.com/package/dotenv) to use environment variables, the [bcrypt package](https://www.npmjs.com/package/bcrypt) to hash passwords, and the [express-session](https://www.npmjs.com/package/express-session) and [connect-session-sequelize](https://www.npmjs.com/package/connect-session-sequelize) packages to add authentication.

* The [express-session](https://www.npmjs.com/package/express-session) package is required to store the session data on the client in a cookie. When the user is idle on the site for more than a set time, the cookie will expire and the user will be required to log in again to start a new session. This is the default behavior and nothing is to be done except to include the implementation of the package.

  - npm install express
  - npm install --save mysql2
  - npm i sequelize
  - npm install dotenv --save
  - npm i bcrypt 
  - npm install express-session
  - npm i connect-session-sequelize
  - npm i handlebars
  - npm i express-handlebars

* Nodemon is installed as development dependency meaning that if our application ever goes in production, this package will not be included. The command to install for in this case is npm i -D nodemon. The purpose of this package is to watch for any changes in our files and restart the server instead of us having to do that manually ourselves. The screenshot show the working of the nodemon.  

* The test of the application is done locally before deployment to Heroku using Insomnia.  At the command prompt, type in npm start or nodemon server.js:-

  ![alt text](/assets/img15.png)

* Testing locally using Insomnia

  ![alt text](/assets/img08.png)

* The database models are set up in accordance to the criteria.   MySQL Workbench is installed to help with design, create and browse the database schemas, work with database objects and insert data as well as design and run SQL queries to work with stored data.  Schemas and data from other database vendors can be migrated from database vendors to MySQL database.
  
* For this application, at command prompt, type in node seeds/index.js :- 

   ![alt text](/assets/img21.png)

* Below shows MySQL Workbench for the database, tech_blog:-

    ![alt text](/assets/img09.png)
    ![alt text](/assets/img10.png)
    ![alt text](/assets/img11.png)
    ![alt text](/assets/img12.png)

## Usage

The steps to show on how the user could use the tech-blog:-

* This application is deployed to Heroku,  click on the link  [HEROKU - THE TECH BLOG](https://stark-tor-51492.herokuapp.com/).

* When the user visit the CMS-style Blog site, the user will be presented with the home page, which includes the existing blog posts, navigation links for the homepage.

  ![alt text](/assets/img14.png)

* When the user is taken to the homepage and clicking on any other links in the navigation, the user would be prompted to either sign up or sign in.  When the user choose to sign up and prompted to create a username and password and click on the sign-up button, the user credentials are saved and the user is logged into the site.

   ![alt text](/assets/img02.png)
   ![alt text](/assets/img03.png)
   ![alt text](/assets/img01.png)


* When the user revisit the site at a later time and choose to sign in, the user is prompted to enter the username and password, and signed into the site, the user can see the navigation links for the homepage, the dashboard, and the option to log out.  When the user click on the homepage option in the navigation, the user is taken to the homepage and presented with existing blog posts that include the post title and the date created.

  ![alt text](/assets/img05.png)
  ![alt text](/assets/img04.png)

* When the user click on the existing blog post, the user will be presented with the post title, contents, post creator's username, and date created for that post and have option to comment. When the user enter a comment and click on the submit button while signed in, then the comment is saved and the post is updated to display the coment, the comment creator's username, and the date created.

  ![alt text](/assets/img07.png)

* when the user click on the dashboard option in the navigation, then the user is taken to the dashboard and presented with the blog post the user have created and the option to add a new blog post and when the click on the button (grey bar) to add a new blog post.  Then the user is prompted to enter both a title and contents for the blog post and when the user click on the button to create a new blog post.  The title and contents of the post are saved and the user is taken back to an updated dash board with the new blog post.

  ![alt text](/assets/img16.png)
  ![alt text](/assets/img17.png)
  ![alt text](/assets/img18.png)

* When the user click on one of the existing posts in the dashboard, then the user is able to delete or update the post and taken back to updated dashboard.  When the user click on the logout option in the navigation , then the user is signed out of the site or idle on the site for more than a set time. The user is able to view comments but prompted to log in again before the user can add, update or delete comments.

  ![alt text](/assets/img19.png)
  ![alt text](/assets/img20.png)


## References

 - The Unit Ahead : Model-View-Controller (MVC):-
     * [MVC Tutorial for Beginners](https://www.guru99.com/mvc-tutorial.html)
     * [What is MVC? Simple Explanation](https://www.youtube.com/watch?v=pCvZtjoRq1I)
     * [What is programming MVC](https://www.youtube.com/watch?v=1IsL6g2ixak)
     * [Separation of Concerns](https://www.youtube.com/watch?v=iO1mnztmqJ8)
     * [Templating languages: The hidden costs - Fun Fun Function](https://www.youtube.com/watch?v=EmGfdlixQHo)
- Unit 14: Student Mini Project - Crowdfunding App
- Request - Response The Full-Stack Blog : Heroku Deployment Guide

## License

This project is licensed under the terms of the MIT license.