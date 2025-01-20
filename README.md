Nodejs template anyone can use to start their project, If you want to make any changed feel free to do it.



`src` -> Inside src folder all actual source code ragarding the project will reside, this will nt include any type of tests. You might can create separate test folder.

Lets have a look at `src` folder:

-`config` -> In this folder anything regarding any configuration or setup of a library or module can be done.It also include log file to prepare meaningful logs.


-`routes` ->In routes folder we register our routes and corresponding middlewares and controllers.


-`middlewares`  -> They are just for intercepting incomming request for writing validators, authenticators, etc.



-`controllers` -> Folder for writing the actual business logic.


-`repositories` ->It contain all the logics using which we interact with the DB by writing queries or ORM queries.


-`services` ->It also contain the business logics and  interfaces with repositories for data from database.






Insided `src/config` then, create a new config.json  file and write these code and fill your username, password, dbname, etc;



        ```
{
  "development": {
    "username": "root",
    "password": null,
    "database": "database_development",
    "host": "127.0.0.1",
    "dialect": "mysql"
  },
  "test": {
    "username": "root",
    "password": null,
    "database": "database_test",
    "host": "127.0.0.1",
    "dialect": "mysql"
  },
  "production": {
    "username": "root",
    "password": null,
    "database": "database_production",
    "host": "127.0.0.1",
    "dialect": "mysql"
  }
}
   ```



Do setting if you are in development mode with the informations that needed.