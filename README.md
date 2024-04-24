# E-Commerce Back End (ORM)

## Description 

The aim of this project is to create a back-end for an e-commerce site. The video link in the links section demonstrates the workings and functionality of the e-commerce back end that was configured with Express.js API and the use of Sequelize to interact with a PostgreSQL database.  

## Table of Contents 

* [Criteria](#criteria)
* [Usage](#usage)
* [Built With](#built-with)
* [Links](#links)

## Criteria

```md
GIVEN a functional Express.js API
WHEN I add my database name, PostgreSQL username, and PostgreSQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the PostgreSQL database
WHEN I open API GET routes in Insomnia for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia
THEN I am able to successfully create, update, and delete data in my database
```

## Usage 

* Use 'pg' and 'sequelize' packages to connect your Express.js API to the PostgreSQL database and the 'dotenv' package to use environment variables to store sensitive data - to do this run 'npm i'
* Populate the environment variable file with the database name and your Postgres username and password. 
* Login to Postgres by running 'psql -U postgres' in the terminal and then insert your Postgres password. To read in the commands from the 'schema' file and create the ecommerce database, you will run '\i db/schema.sql'.
* Once database has been created, exit postgres using '\q' and then run 'node seeds/index.js' in the terminal to populate the database with test data.
* Run 'npm start' to start the server for the Sequelize models to be synced to the PostgreSQL database  
* Using Postman, open the API GET routes for products, categories and tags and they appropriate data for each route should be displayed in JSON format. 
* Then create, update and delete data corresponding to products, categories and tags using the API POST, PUT and DELETE routes.

## Built With 

* Inquirer (npm utility)
* Express.js
* Node.js
* Sequelize
* PostgreSQL 

## Links 

Link to Demonstration Video - https://youtu.be/X9aRTza6CBA 