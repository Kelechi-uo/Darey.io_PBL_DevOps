<!-- BASIC EXPLANATION OF SOFTWARE DEVELOPMENT LIFE CYCLE (SDLC) -->

## What is SDLC?

### SDLC stands for Software Development Life Cycle, which is a process that outlines the steps involved in creating software from conception to deployment. The process is designed to ensure that the software is developed according to the specific requirements and that the final product is of high quality. The main steps involved in the SDLC are:

1. Requirements gathering and analysis: This involves understanding the needs of the customers and stakeholders, and determining the requirements for the software.

2. Design: In this phase, the software architecture and design are developed, including the selection of the appropriate technology and tools.

3. Implementation: This is the actual coding and development of the software, where the design is turned into a working product.

4. Testing: In this phase, the software is thoroughly tested to ensure that it meets the specified requirements and works as expected.

5. Deployment: After the software has been thoroughly tested, it is deployed to the production environment and made available to the end-users.

6. Maintenance: This is an ongoing process that involves fixing bugs, making improvements, and updating the software to keep it current and functional.

The SDLC provides a structured approach to software development and helps to ensure that the software is delivered on time, within budget, and to the required quality.

---

<!-- BASIC EXPLANATION OF LAMP -->

## What is LAMP?

### LAMP is an acronym that stands for Linux, Apache, MySQL, and PHP. It refers to a software stack that is used to build dynamic websites and web applications. The components of the LAMP stack are:

1. Linux: A free and open-source operating system that is the foundation of the LAMP stack.

2. Apache: An open-source web server software that is used to serve web pages and run web applications.

3. MySQL: A popular open-source relational database management system used to store and manage data for websites and web applications.

4. PHP: A server-side scripting language used to build dynamic websites and web applications. It is used to write scripts that interact with databases, generate HTML pages, and perform other tasks.

Together, these components form a complete solution for building and running web applications. The LAMP stack is popular because it is open-source, flexible, and provides a cost-effective solution for small and medium-sized businesses. It is also scalable, meaning that it can grow with a business's needs.

--- 

<!-- BASIC EXPLANATION OF CHMOD -->

## WHAT is chmod?

chmod is a command in Unix-like operating systems that stands for "change mode" and is used to change the permissions on a file or directory. Permissions determine which users have access to read, write, or execute a file or directory.

**Key take away:** 

Chmod takes three main arguments: `r`, `w`, and `x`, which stand for read, write, and execute, respectively. Adding or removing combinations of the arguments controls file and folder permissions. For example, `chmod +rwx` adds permission to read, write, and execute scripts. Running `chmod -wx` removes the ability to write and execute.

**chmod Modifies File Permissions:**

In Linux, who can do what to a file or directory is controlled through sets of permissions. There are three sets of permissions. One set for the owner of the file, another set for the members of the file’s group, and a final set for everyone else.

The permissions control the actions that can be performed on the file or directory. They either permit, or prevent, a file from being read, modified or, if it is a script or program, executed. For a directory, the permissions govern who can cd into the directory and who can create, or modify files within the directory.

**Viewing and Understanding File Permissions**

We can use the `-l` (long format) option to have `ls` list the file permissions for files and directories.

    ls -l

The output will look like this below

![Alt text](Images/Ls%20-L.png)

On each line, the first character identifies the type of entry that is being listed. If it is a dash `-` it is a file. If it is the letter `d` it is a directory.

The next nine characters represent the settings for the three sets of permissions.

* The first three characters show the permissions for the user who owns the file (user permissions).

* The middle three characters show the permissions for members of the file’s group (group permissions).

* The last three characters show the permissions for anyone not in the first two categories (other permissions).

There are three characters in each set of permissions. The characters are indicators for the presence or absence of one of the permissions. They are either a dash `-` or a letter. If the character is a dash, it means that permission is not granted. If the character is an `r`, `w`, or an `x`, that permission has been granted.

The letters represent:

* `r`: Read permissions. The file can be opened, and its content viewed.

* `w`: Write permissions. The file can be edited, modified, and deleted.

* `x`: Execute permissions. If the file is a script or a program, it can be run (executed).



