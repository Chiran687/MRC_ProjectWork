<h1>PHP CRUD Operations with Dockerized MySQL Database.</h1>

This repository demonstrates a simple PHP CRUD (Create, Read, Update, Delete) application using Docker Compose to set up a MySQL container. The application utilizes PDO (PHP Data Objects) for database operations.

Files:

config.php: Configuration file containing database connection details.

create.php: Create operation - Add new records to the database.

delete.php: Delete operation - Remove records from the database.

error.php: Error page - Displayed in case of any errors during operations.

index.php: Main page - Displaying the list of records and navigation options.

read.php: Read operation - Fetch and display records from the database.

update.php: Update operation - Modify existing records in the database.

Docker Configuration
docker-compose.yml: Docker Compose configuration file to set up a MySQL container.

Usage
1. Clone the repository:
    https://github.com/Chiran687/MRC_ProjectWork.git
2. Navigate to the project directory:
   cd PHP_CRUD
3. Run docker-compose file:
   docker-compose up -d
4. Enable PDO extension in php.ini
5. Run PHP local server:
   php -S 127.0.0.1:8000
6. Access the application in your browser:
   http://localhost:8080

   
Even though the curriulum of BICTE third semester used Mysqli, I am using PDO because of many advandatges of PDO over MySQLi.

Advantages of PDO over MySQLi

1. Database Support:
PDO: Supports multiple databases, including MySQL, PostgreSQL, SQLite, and others. Allows easier database migration.
MySQLi: Primarily designed for MySQL databases.

2. Named Placeholders:
PDO: Supports named placeholders in queries, making code more readable.
MySQLi: Uses "?" as placeholders, which can be less expressive.

3. Object-Oriented Interface:
PDO: Provides an object-oriented interface, making it easier to work with.
MySQLi: Offers both procedural and object-oriented interfaces.


4. Error Handling:
PDO: Provides a consistent error-handling approach, allowing exception handling.
MySQLi: Requires explicit error checking using functions like mysqli_error.

5. Security:
PDO: Provides a higher level of security with prepared statements, reducing the risk of SQL injection.
MySQLi: Also supports prepared statements but may require additional steps for proper usage.

6. Database Abstraction:
PDO: Acts as a database abstraction layer, facilitating code portability between different databases.
MySQLi: Tightly coupled with MySQL-specific features.

7. Ease of Use:
PDO: Simplifies code by providing a unified API for different databases.
MySQLi: Requires more code for certain operations and lacks consistency in some aspects.

Choose PDO or MySQLi based on your project requirements and preferences. PDO is often favored for its flexibility and support for multiple databases.
