# Node.js Microservice Template

A template for creating REST microservices using Node.js

## Table of Contents
* [General info](#general-info)
* [App Stack](#app-stack)
  * [Backend](#backend)
  * [Frontend](#frontend)
  * [Mobile App](#mobile-app)
* [Setting it Up](#setting-it-up)

## General Info
**_Disclaimer: this is a work in progress._**

The template have been implemented using [Express](https://expressjs.com), which is a fast, minimalist web framework for Node.js, alongside [Knex](https://knexjs.org) to handle database migrations.

Unit tests and integration tests were implemented using [Jest](https://jestjs.io) and supertest

### Setting it Up
```
$ yarn install
```

### Start the service
And then, we start the services:

```
$ yarn start
```

### DB Migrations
To create migration files, run:
```
$ yarn run knex migrate:make <file_name>
```

To run the migrations (in the first time, it creates the sqlite3 database in dev and test), run:
```
$ yarn run knex migrate:make
```