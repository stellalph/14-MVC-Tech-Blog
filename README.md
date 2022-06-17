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

## Usage

## References

## License

This project is licensed under the terms of the MIT license.