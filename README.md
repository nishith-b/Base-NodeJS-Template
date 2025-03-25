This is a Base NodeJs Project template, which anyone can use as it has been prepared, by keeping some of the most important code principles and project management recommendations.Feel Free to change anything.


`src` -> Inside the src folder all the actual source code regarding the project will reside, this will not include any kind of tests.(You might wnat to make seperate tests folder)

Lets take a look inside the `src` folder

- `config` -> In this floder anything and everything regarding any configurations or setup of a library or module will be done. for example: setting up `dotenv` so that we can use the environment variables in a cleaner fashion.this is done in the `server-config.js`. One more example is to setup logging library that can help to prepare meaning full logs.so, configuration for this library also done here.


### Setup the Project

    -Download



    -Inside the `src/config/` create file named  `config.json` and write the follwoing code:

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

-go inside the `src` folder and execute the following command
  npx sequelize init

- If you're setting up your dev environment set up username and password of your db and mention db name in dialect.do same for test and prod env

