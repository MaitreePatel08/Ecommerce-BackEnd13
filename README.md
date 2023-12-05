# Ecommerce-BackEnd13

# Description

This project offers the (almost) complete back end of an inventory management app for a small online retail store. By carefully defining the basic routes that such an API would possess, we give potential users the flexibility of adding additional routes and implementing the front end that will serve them best. We divide the routes into three types, each corresponding to a JS class: categories, products and tags. The classes have the following pairwise relations:

1. Each product belongs to a category.

2. Categories serve to classify many products.

3. For each product there are various tags attached to it, describing some feature they have.

4. Each tag can be attached to many products.

With the purpose of showing functionality, some seeding files were included as part of the package to be used as sample data.

Considered as an exercise in coding, this projects allows to practice using packages such as:

1. "DotEnv" to define environemental variables that protect sensitive configuration information that will vary among deployments.

2. "Express.js" in order to be able to instantiate a server and routers for the GET, POST, PUT, and DELETE routes defined for each endpoint.

3. "Sequelize" to use ORM, synchronizing models (implemented as JS classes) to the database and make queries to it using scripts instead of SQL statements.

We have continued developing the modularization/separation of concerns that have been one of the pillars of our incursion into back end development within the Node runtime environment and practice defining RESTful routes.


# Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)


# Installation

1. Go to the CLI of Git BASH and use the "mkdir" command to create a new directory for the folder. Use the "cd" command to change directory.

2. Navigate to <https://github.com/MaitreePatel08/Ecommerce-BackEnd13.git>, press the "<> Code" button, choose the most convenient way to clone the repo, and copy the direction.

3. Go back to Git BASH and append the copied direction to the command "git clone" .

4. Enter whathever means of authorization (e.g. a passphrase for SSH Keys) they ask you.

5. Once cloning is done, go to the MySQL Shell in order to run the command "SOURCE db/schema.sql;". That will create the new database for you.

6. Change the name of the "$.env.Example" file to .env and save the data needed to create a "sequelize" configuration in the environmental variables whose identifiers are provided in the file.

7. Within Git BASH, run "npm install" to install the dependencies in the package.json file.

8. Enter "npm run seed" in order to seed the database, i.e., create the tables onto which the Sequelize models map and populate them.

9. Enter "npm start" so as to synchronize the Sequelize models with the ecommerce_db and have the Express server listening at the port stipulated in the "server.js" file. Once the message
"App listening on port ${port}!" appears in the terminal, you can start testing the routes, some of them in the browser of your choice while others will require an API platform like"PostMan"/"Insomnia".
