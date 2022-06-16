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

* The application follows the Model-View-Controller paradigm.  The Model-View-Controller(MVC) framework is an architectural pattern that adheres to the separation of concerns principle.

* The folder structure for the application will be set up to MVC paradigm.

  - The Model - stores data and data-related logic
  - The View - the UI/UX concerns, or what a user will see and interact with.
  - The Controller - the interface between Models and Views.  It processes requests from the View, uses the Model to 
    manipulate data, and sends data to the View to render.

* This application will need the installation of node.js from the website, https://www.node.org.

* Node Package Manager (npm) is a software manager and installer which puts the modules in place so that the node project can utilize it, and also, it manages dependency conflicts intelligently and initialized using <strong>npm init</strong>.  The package.json will be generated and will contains all the details of the application in which the user have inputted during the npm initialization.

* This application also need the installation of MySQL which is a developer-friendly open source relational databse system.  The application uses MySQL packjage and sequelize package to connect Express.js to MySQL database and also the dotenv package to use environment variables to store sensitive data. Dotenv is a zero-dependency module that loads environment variables from a .env file into process.env. The bcrypt package is to hash passwords, and the express-session and connect



  - npm install express
  - npm install --save mysql2
  - npm i sequelize
  - npm install dotenv --save
  - npm i bcrypt 

* Nodemon is installed as development dependency meaning that if our application ever goes in production, this package will not be included. The command to install for in this case is npm i -D nodemon. The purpose of this package is to watch for any changes in our files and restart the server instead of us having to do that manually ourselves. The screenshot show the working of the nodemon.  



## Usage

## References

## License
