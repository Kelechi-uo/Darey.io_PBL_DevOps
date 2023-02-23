
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

<!-- WEB STACK IMPLEMENTATION (LEMP STACK) -->

<!-- Step 1 - Installing the Nginx web server -->

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

Before we can receive any traffic by our Web Server, we need to open TCP port 80 which is default port that web browsers use to access web pages in the Internet.

As we know, we have TCP port 22 open by default on our EC2 machine to access it via SSH, so we need to add a rule to EC2 configuration to open inbound connection through port 80:

Our server is running and we can access it locally and from the Internet (Source 0.0.0.0/0 means ‘from any IP address’).

First, let us try to check how we can access it locally in our Ubuntu shell, run:

    curl http://localhost:80
  
or

    curl http://127.0.0.1:80 

Nginx responded with some payload, see image below:

![Alt text](Project2_images/nginx%20loading.png)

These 2 commands above actually do pretty much the same – they use ‘curl’ command to request our Nginx on port 80 (actually you can even try to not specify any port – it will work anyway). The difference is that: in the first case we try to access our server via DNS name and in the second one – by IP address (in this case IP address 127.0.0.1 corresponds to DNS name ‘localhost’ and the process of converting a DNS name to IP address is called "resolution"). We will touch DNS in further lectures and projects.

As an output you can see some strangely formatted test, do not worry, we just made sure that our Nginx web service responds to ‘curl’ command with some payload.

Now it is time for us to test how our Nginx server can respond to requests from the Internet.
Open a web browser of your choice and try to access following url

    http://<Public-IP-Address>:80

Another way to retrieve your Public IP address, other than to check it in AWS Web console, is to use following command:

    curl -s http://169.254.169.254/latest/meta-data/public-ipv4

The URL in browser shall also work if you do not specify port number since all web browsers use port 80 by default.

If you see following page, then your web server is now correctly installed and accessible through your firewall.

page loaded succesfully, see image below:

![Alt text](Project2_images/nginx%20loaded%20on%20browser.png)

In fact, it is the same content that you previously got by ‘curl’ command, but represented in nice HTML formatting by your web browser.


<!-- STEP 2 - Installing MYSQL -->

## STEP 2 — INSTALLING MYSQL

Now that you have a web server up and running, you need to install a Database Management System (DBMS) to be able to store and manage data for your site in a relational database. MySQL is a popular relational database management system used within PHP environments, so we will use it in our project.

Again, use ‘apt’ to acquire and install this software:

    sudo apt install mysql-server

When prompted, confirm installation by typing `Y`, and then `ENTER`.

MYSQL insatllation completed, see image below:
![Alt text](Project2_images/mysql%20install.png)

When the installation is finished, log in to the MySQL console by typing:  

    sudo mysql

This will connect to the MySQL server as the administrative database user root, which is inferred by the use of sudo when running this command. You should see output like this:

    Welcome to the MySQL monitor.  Commands end with ; or \g.
    Your MySQL connection id is 11
    Server version: 8.0.22-0ubuntu0.20.04.3 (Ubuntu)

    Copyright (c) 2000, 2020, Oracle and/or its affiliates. All rights reserved.

    Oracle is a registered trademark of Oracle Corporation and/or its
    affiliates. Other names may be trademarks of their respective
    owners.

    Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

    mysql> 

It’s recommended that you run a security script that comes pre-installed with MySQL. This script will remove some insecure default settings and lock down access to your database system. Before running the script you will set a password for the root user, using mysql_native_password as default authentication method. We’re defining this user’s password as `PassWord.1`

    ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'PassWord.1';

Exit the MySQL shell with:

    mysql> exit

Start the interactive script by running:

    sudo mysql_secure_installation

This will ask if you want to configure the VALIDATE PASSWORD PLUGIN.

Note: Enabling this feature is something of a judgment call. If enabled, passwords which don’t match the specified criteria will be rejected by MySQL with an error. It is safe to leave validation disabled, but you should always use strong, unique passwords for database credentials.

Answer `Y` for yes, or anything else to continue without enabling.

    VALIDATE PASSWORD PLUGIN can be used to test passwords
    and improve security. It checks the strength of password
    and allows the users to set only those passwords which are
    secure enough. Would you like to setup VALIDATE PASSWORD plugin?

    Press y|Y for Yes, any other key for No:

If you answer “yes”, you’ll be asked to select a level of password validation. Keep in mind that if you enter `2` for the strongest level, you will receive errors when attempting to set any password which does not contain numbers, upper and lowercase letters, and special characters, or which is based on common dictionary words e.g `PassWord.1`

    There are three levels of password validation policy:

    LOW    Length >= 8
    MEDIUM Length >= 8, numeric, mixed case, and special characters
    STRONG Length >= 8, numeric, mixed case, special characters and dictionary              file

    Please enter 0 = LOW, 1 = MEDIUM and 2 = STRONG: 1

Regardless of whether you chose to set up the VALIDATE PASSWORD PLUGIN, your server will next ask you to select and confirm a password for the MySQL root user. This is not to be confused with the system root. The database root user is an administrative user with full privileges over the database system. Even though the default authentication method for the MySQL root user dispenses the use of a password, even when one is set, you should define a strong password here as an additional safety measure. We’ll talk about this in a moment.

If you enabled password validation, you’ll be shown the password strength for the root password you just entered and your server will ask if you want to continue with that password. If you are happy with your current password, enter `Y` for “yes” at the prompt:  

    Estimated strength of the password: 100 
    Do you wish to continue with the password provided?(Press y|Y for Yes, any other key for No) : y

For the rest of the questions, press `Y` and hit the `ENTER` key at each prompt. This will prompt you to change the root password, remove some anonymous users and the test database, disable remote root logins, and load these new rules so that MySQL immediately respects the changes you have made.

When you’re finished, test if you’re able to log in to the MySQL console by typing:

    sudo mysql -p

Notice the `-p` flag in this command, which will prompt you for the password used after changing the root user password.

To exit the MySQL console, type:  

    mysql> exit

Notice that you need to provide a password to connect as the root user.

For increased security, it’s best to have dedicated user accounts with less expansive privileges set up for every database, especially if you plan on having multiple databases hosted on your server.

    Note: At the time of this writing, the native MySQL PHP library mysqlnd doesn’t support caching_sha2_authentication, the default authentication method for MySQL 8. For that reason, when creating database users for PHP applications on MySQL 8, you’ll need to make sure they’re configured to use mysql_native_password instead. We’ll demonstrate how to do that in Step 6.

Your MySQL server is now installed and secured. Next, we will install PHP, the final component in the LEMP stack.    









