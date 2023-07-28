# Sql-Command-and-Use
<html>
   <head>
        <title> Sql Command & Use </title>
        <style>

            body{
                background-color: pink ;
                background-repeat: repeat;
            }

            table {
                border-collapse: separate;
                text-indent: initial;
                border-spacing: 2px;
            }

            h1{
                text-align: center;
                color: red;
            }

            h3{
                color: red;
                font-style: italic;
            }

            li{
                color: blue;
            }

            pre{
               font-family: serif; 
            }

        </style>
   </head>
        <body>
            <h1> Sql command thear typs and use </h1> <hr>
        
            <h2> SQL commands are used to interact with a database. There are five main types of SQL commands: </h2>
        <ol>
            <li> Data Definition Language (DDL): DDL commands are used to create, modify, and delete database objects, such as tables, views, and indexes.</li>
            <li> Data Manipulation Language (DML): DML commands are used to insert, update, and delete data from tables.</li>
            <li> Data Control Language (DCL): DCL commands are used to manage user permissions and privileges.</li>
            <li> Transaction Control Language (TCL): TCL commands are used to manage transactions, which are a set of DML statements that are executed together as a single unit.</li>
            <li> Data Query Language (DQL): DQL commands are used to retrieve data from tables.</li>
        </ol>

<hr>
            <h2> Here are some of the most important SQL commands: </h2>
        <ol>
            <li> CREATE TABLE: Creates a new table. </li>
        <h3> Syntax: </h3>
            <pre> CREATE TABLE table_name (
        column1 datatype,
        column2 datatype,
        column3 datatype,
        columnN datatype
        ); </pre>

        <h3> Example: </h3>
            <pre> CREATE TABLE pets (
        name VARCHAR(20),
        owner VARCHAR(20),
        species VARCHAR(20),
        sex CHAR(1)
         ); </pre>
                       
<hr>
         <li> INSERT INTO: Inserts a new row into a table. </li>
        <h3> Syntax: </h3>
            <pre> INSERT INTO table_name (column1, column2, column3, ...)
        VALUES (value1, value2, value3, ...); </pre>

        <h3> Example: </h3>
            <pre> INSERT INTO pets (name, owner, species, sex)
        VALUES ('Spot', 'John Doe', 'Dog', 'M'); </pre>
            
<hr>
            <li> SELECT: Retrieves data from a table. </li>
        <h3> Syntax: </h3> 
            <pre> SELECT column1, column2, column3, ...
        FROM table_name </pre>
        
        <h3> Example: </h3>
            <pre> SELECT name, owner, species
        FROM pets; </pre>
            
<hr>
            <li> UPDATE: Updates data in a table. </li>
        <h3> Syntax: </h3>
            <pre> UPDATE table_name
        SET column1 = value1, column2 = value2, ...
        WHERE condition; </pre>

        <h3> Example: </h3>    
            <pre> UPDATE pets
        SET species = 'Cat'
        WHERE name = 'Spot'; </pre>
            
<hr>
            <li> DELETE: Deletes data from a table. </li>
        <h3> Syntax: </h3>
            <pre> DELETE FROM table_name
        WHERE condition; </pre>
        
        <h3> Example: </h3>
            <pre> DELETE FROM pets
        WHERE species = 'Dog'; </pre>
    
<hr>
            <li> GRANT: Grants permissions to users. </li>
        <h3> Syntax: </h3>
            <pre> GRANT privilege_list ON object_name TO user_name [WITH GRANT OPTION]; </pre>
        
        <h3> Example: </h3>
            <pre> GRANT SELECT, UPDATE ON pets TO johndoe; </pre>
            
<hr>
            <li> REVOKE: Revokes permissions from users. </li>
        <h3> Syntax: </h3>
            <pre> REVOKE privilege_list ON object_name FROM user_name; </pre>
        
        <h3> Example: </h3>
            <pre> REVOKE SELECT, UPDATE ON pets FROM johndoe; </pre>

<hr>
            <li> COMMIT: Commits a transaction. </li>
        <h3> Syntax: </h3> 
            <pre> COMMIT; </pre>

        <h3> Example: </h3>    
            <pre> UPDATE pets
        SET species = 'Cat'
        WHERE name = 'Spot';
        COMMIT; </pre>

<hr>            
            <li> ROLLBACK: Rolls back a transaction. </li>
        <h3> Syntax: </h3>
            <pre> ROLLBACK; </pre>
        
        <h3> Example: </h3>
            <pre> UPDATE pets
        SET species = 'Cat'
        WHERE name = 'Spot';
        ROLLBACK; </pre>
        </ol>      
<hr>      
    </body>
</html>
