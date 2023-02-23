
# PROJECT 2 - WEB STACK IMPLEMENTATION (LEMP STACK)

## SIDE SELF STUDY:

<!-- Basic explanation of SQL syntax and most commonly used commands -->

## What is SQL?

SQL (Structured Query Language) is a programming language used for managing and manipulating relational databases. Here are some of the most commonly used SQL commands and syntax:

1. SELECT - used to retrieve data from a database. Syntax:
SELECT column_name(s) FROM table_name WHERE condition;

2. INSERT - used to insert new records into a table. Syntax:
INSERT INTO table_name (column1, column2, column3, ...) VALUES (value1, value2, value3, ...);  

3. UPDATE - used to update existing records in a table. Syntax:
UPDATE table_name SET column1 = value1, column2 = value2 WHERE condition; 

4. DELETE - used to delete records from a table. Syntax:
DELETE FROM table_name WHERE condition;   

5. CREATE - used to create a new table, index, or view. Syntax:
CREATE TABLE table_name (column1 datatype, column2 datatype, column3 datatype, ...);

6. ALTER - used to modify the structure of an existing table. Syntax:
ALTER TABLE table_name ADD column_name datatype; 

7. DROP - used to drop a table or database object. Syntax:
DROP TABLE table_name;   

8. JOIN - used to combine data from two or more tables. Syntax:
SELECT column_name(s) FROM table1 INNER JOIN table2 ON table1.column_name = table2.column_name; 

9. WHERE - used to filter data based on a specified condition. Syntax:
SELECT column_name(s) FROM table_name WHERE condition;    

10. ORDER BY - used to sort the result set in ascending or descending order
Syntax:
SELECT column_name(s) FROM table_name ORDER BY column_name ASC/DESC;

These are just a few examples of SQL syntax and commands. SQL has many other commands and features, depending on the database management system (DBMS) you are using. For more details and practice click [here](https://www.w3schools.com/sql/sql_syntax.asp)


# Web stack (LEMP) implimentation in AWS

## STEP 1 – INSTALLING THE NGINX WEB SERVER

In order to display web pages to our site visitors, we are going to employ Nginx, a high-performance web server. We’ll use the apt package manager to install this package.

Since this is our first time using apt for this session, start off by updating your server’s package index. Following that, you can use apt install to get Nginx installed:

To update the package lists, run the following command: 
    
    sudo apt update

To upgrade the installed packages to their latest versions, run following command: 

    sudo apt upgrade

You can view the list of upgraded packages after running the `sudo apt upgrade` command by using the `apt list --upgradable` command. This command will show you a list of all packages that have updates available, including the ones that were upgraded during the most recent `apt upgrade` command.

To view the list of upgraded packages, open a terminal on your server and run the following command: 

    apt list --upgradable

This will display a list of all available upgrades, including the package name, the current installed version, and the version to which the package will be upgraded. The upgraded packages will be marked with the `[upgradable]` tag.

If you want to see only the list of packages that were upgraded during the most recent upgrade process, you can use the following command: 

    grep -i "upgrade" /var/log/dpkg.log

Server packages updated, see image below

![Alt text](Project2_images/package%20update.png)

To install Nginx, run the following command: 
    
    sudo apt install nginx

To verify that nginx was successfully installed and is running as a service in Ubuntu, run:

    sudo systemctl status nginx

Nginx successfully insatlled, see image below:    

![Alt text](Project2_images/nginx%20installed1.png)

