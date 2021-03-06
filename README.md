# E-Commerce Back End
![Github license](http://img.shields.io/badge/license-MIT-blue.svg)

Created a back end for a general company's e-commerce site using Express.js API and Sequelize configurations to interact with a MySQL database.

## Table of Contents

* [Setup](#setup)
* [Usage](#usage)
* [Contributing](#contributing)
* [License](#license)

## Setup
:floppy_disk:

Either clone, fork and follow the following instructions to use your own package.json and package-lock.json.

[Node's website](https://nodejs.org/en/) and follow the download instructions for your appropriate setup. NPM, or Node Package Manager, is the default package manager for Node.js. It is distributed with Node.js.

The database uses the following npm:
- [Node Package Manager](https://nodejs.org/en/)
  - Run `npm install` in order to install the following npm package dependencies as specified in the `package.json`.
  - This will also help install express on your system and manage any other dependencies in your script.
- [Express](https://www.npmjs.com/package/express)
  - Express is a back end web application framework for Node.js. Released as free and open-source software under the MIT License. Designed for building web applications and APIs. Many users use it as a standard server framework for Node.js.
- [dotenv](https://www.npmjs.com/package/dotenv)
  - A Zero-dependency module that loads environment variables from a `.env` file into `process.env`.

Uses the following SQLs:
- [MySQL](https://www.mysql.com/)
  - Considered the most reliable, scaleable, and developer-friendly open source relational dtabase management system. It powers the back end of many popular social, streaming, and service web applications.
- [MySQL2](https://www.npmjs.com/package/mysql2)
  - An npm package for Node.js with a focus on performance. Connects Node.js applications to the MySQL database.

This database uses Insomnia to test and manipulate data:

- [Insomnia](https://insomnia.rest/)
  - Delivers APIs to send REST, SOAP, GraphQL, and GRPC requests directly within Insomnia.

`npm init`

`npm install express`

`npm install dotenv`

`npm install --save mysql2`

Ensure that you create an .env file in your local repository with similar text below before using:
```js
DB_NAME='ecommerce_db'
DB_USER='your-username' // typically root
DB_PW='your-password'
```

## Usage

:computer:

To start, ensure that you create the schema from the MySQL shell through the terminal:

`mysql -u root -p`

Enter your password and create the database:

`CREATE DATABASE ecommerce_db;`

Switch to your regular powershell terminal and run the following command line prompts:

`npm run seed` to seed data to your database.

`npm start` or `node server.js` to start the server.

![!demo gif](./assets/ecommerce_create_schema.gif)

Open Insomnia to be able to test the data provided.

Below is a demonstration of `CATEGORIES` routes for `GET`, `GET` by ID, `POST`, `PUT` (update) and `DELETE`.

![!demo gif](./assets/ecommerce_categories_demo.gif)

Below is a demonstration of `PRODUCTS` routes for `GET`, `GET` by ID, `POST`, `PUT` (update) and `DELETE`.

![!demo gif](./assets/ecommerce_products_demo.gif)

Below is a demonstration of `TAGS` routes for `GET`, `GET` by ID, `POST`, `PUT` (update) and `DELETE`.

![!demo gif](./assets/ecommerce_tags_demo.gif)

## Contributing

:octocat:

[paperpatch](https://github.com/paperpatch)

## License

:receipt:

This project is licensed under MIT.