# e-commerce

## Description
This is a functional Express.js API that uses Sequelize as an Object-Relational Mapping (ORM) tool to interact with a MySQL database. It provides routes to perform various CRUD (Create, Read, Update, Delete) operations on categories, products, and tags.

## Installation and Setup
To get started with this Express.js API, follow these steps:

Clone the repository to your local machine.

Create an environment variable file (.env) in the root directory of the project and add the following variables:

makefile
Copy code
DB_NAME=your_database_name
DB_USER=your_mysql_username
DB_PASSWORD=your_mysql_password
Replace your_database_name, your_mysql_username, and your_mysql_password with your actual MySQL database credentials.

Open a terminal and navigate to the project directory.

Run the following commands to set up the database schema and seed data:
npm i 
npm run schema
npm run seed
This will create a development database and populate it with test data.

Finally, start the application by running:

sql
npm start
This will start the server and sync the Sequelize models with the MySQL database.

## Usage
API Routes
To view data for categories, products, or tags, use API GET routes in tools like Insomnia Core. The data for each route will be displayed in a formatted JSON format.

You can test API POST, PUT, and DELETE routes in Insomnia Core to create, update, and delete data in the database.

## Example API Routes
GET /api/categories: Retrieve a list of all categories.
GET /api/products: Retrieve a list of all products.
GET /api/tags: Retrieve a list of all tags.
POST /api/categories: Create a new category.
POST /api/products: Create a new product.
POST /api/tags: Create a new tag.
PUT /api/categories/:id: Update a category by ID.
PUT /api/products/:id: Update a product by ID.
PUT /api/tags/:id: Update a tag by ID.
DELETE /api/categories/:id: Delete a category by ID.
DELETE /api/products/:id: Delete a product by ID.
DELETE /api/tags/:id: Delete a tag by ID.

## License
This project is licensed under the MIT License.

## Technologies Used
Express.js
Sequelize (ORM)
MySQL
Node.js