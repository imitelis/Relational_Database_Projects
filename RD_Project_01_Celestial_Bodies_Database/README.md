# freeCodeCamp - Relational Database - Projects - I - Celestial Bodies Database


## 1. Projects - Build a Celestial Bodies Database

This is one of the required projects to earn your certification. For this project, you will build a database of celestial bodies using PostgreSQL.

[Create a GitHub](https://github.com/join) account if you don't have one. You'll need it when you create the virtual Linux server machine. This process may take a few minutes.

Complete both steps below to finish the challenge.

### Step 1: Complete the project

The project runs in a virtual machine, complete the user stories described in there and get all the tests to pass to finish step 1.

**Important:** After you pass all the project tests, save a dump of your database into a `universe.sql` file so you can complete step 2. There will be instructions how to do that within the virtual machine.

### Step 2: Submit your code

When you have completed the project, save all the required files into a public repository and submit the URL to it below.

Required files: `universe.sql`

## Instructions

For this project, you need to log in to PostgreSQL with psql to create your database. Do that by entering `psql --username=freecodecamp --dbname=postgres` in the terminal. Make all the tests below pass to complete the project. Be sure to get creative, and have fun!

**Don't forget to connect to your database after you create it 😄**

Here's some ideas for other column and table names: `description`, `has_life`, `is_spherical`, `age_in_millions_of_years`, `planet_types`, `galaxy_types`, `distance_from_earth`.

**Notes:**
If you leave your virtual machine, your database may not be saved. You can make a dump of it by entering `pg_dump -cC --inserts -U freecodecamp universe > universe.sql` in a bash terminal (not the psql one). It will save the commands to rebuild your database in `universe.sql`. The file will be located where the command was entered. If it's anything inside the `project` folder, the file will be saved in the VM. You can rebuild the database by entering `psql -U postgres < universe.sql` in a terminal where the `.sql` file is.

If you are saving your progress on [freeCodeCamp.org](freecodecamp.org), after getting all the tests to pass, follow the instructions above to save a dump of your database. Save the `universe.sql` file in a public repository and submit the URL to it on [freeCodeCamp.org](freecodecamp.org).

### Complete the tasks below

  *  You should create a database named `universe`
  *  Be sure to connect to your database with `\c universe`. Then, you should add tables named `galaxy`, `star`, `planet`, and `moon`
  *  Each table should have a primary key
  *  Each primary key should automatically increment
  *  Each table should have a `name` column
  *  You should use the `INT` data type for at least two columns that are not a primary or foreign key
  *  You should use the `NUMERIC` data type at least once
  *  You should use the `TEXT` data type at least once
  *  You should use the `BOOLEAN` data type on at least two columns
  *  Each "star" should have a foreign key that references one of the rows in `galaxy`
  *  Each "planet" should have a foreign key that references one of the rows in `star`
  *  Each "moon" should have a foreign key that references one of the rows in `planet`
  *  Your database should have at least five tables
  *  Each table should have at least three rows
  *  The `galaxy` and `star` tables should each have at least six rows
  *  The `planet` table should have at least 12 rows
  *  The `moon` table should have at least 20 rows
  *  Each table should have at least three columns
  *  The `galaxy`, `star`, `planet`, and `moon` tables should each have at least five columns
  *  At least two columns per table should not accept `NULL` values
  *  At least one column from each table should be required to be `UNIQUE`
  *  All columns named `name` should be of type `VARCHAR`
  *  Each primary key column should follow the naming convention `table_name_id`. For example, the `moon` table should have a primary key column named `moon_id`
  *  Each foreign key column should have the same name as the column it is referencing