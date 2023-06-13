# PROJECT 3: SIMPLE TO-DO APPLICATION ON MERN WEB STACK

# Self Study Before Taking on Project 3



## What is MERN stack?

Check source [here](https://www.simplilearn.com/tutorials/mongodb-tutorial/what-is-mern-stack-introduction-and-examples#:~:text=MERN%20stack%20is%20a%20collection,stack%20are%20all%20JS%2Dbased.)

MERN stack is a collection of technologies that enables faster application development. It is used by developers worldwide. The main purpose of using MERN stack is to develop apps using JavaScript only. This is because the four technologies that make up the technology stack are all JS-based. Thus, if one knows JavaScript (and JSON), the backend, frontend, and database can be operated easily. 

## MERN Stack Full Form

MERN Stack is a compilation of four different technologies (MongoDB, Express, React / Redux, and Node.js) that work together to develop dynamic web apps and websites. 

It is a contraction for four different technologies as mentioned below:

1. Database  
**MongoDB** is a NoSQL DBMS where data is stored in the form of documents having key-value pairs similar to JSON objects. MongoDB enables users to create databases, schemas, and tables. It offers the Mongo shell that provides a JS interface for deleting, querying, and updating the records.

2. Backend Framework  
**ExpressJS** is a NodeJS framework that simplifies writing the backend code. It saves you from creating multiple Node modules. For keeping the code precise, ExpressJS offers a range of middleware.

3. Frontend Library  
**ReactJS** is a javascript library that allows the development of user interfaces for mobile apps and SPAs (Single Page Applications). It allows you to code JavaScript and develop UI components. The JS library uses virtual DOM for doing everything.

4. Runtime Environment  
**NodeJS** is an open-source JavaScript runtime environment that allows users to run code on the server. It comes with the node package manager or npm, enabling users to select from a wide selection of node modules or packages. Being developed on the Chrome JavaScript Engine enables Node to execute code faster.


## Why Should You Work With MERN Stack?

There are many good reasons to use the MERN Stack. For example, it allows the creation of a 3-tier architecture that includes frontend, backend, and database using JavaScript and JSON.

MongoDB, which is the base of the MERN stack, is designed to store JSON data natively. Everything in it, including CLI and query language, is built using JSON and JS. The NoSQL database management system works well with NodeJS and thus, allows manipulating, representing, and storing JSON data at every tier of the application.

It comes in a variant called MongoDB Atlas that further eases database management by offering an auto-scaling MongoDB cluster on any cloud provider and with just a few clicks.

Express is a server-side framework that wraps HTTP requests and responses and makes mapping URLs to server-side functions easy. This perfectly complements the ReactJS framework, a front-end JS framework for developing interactive UIs in HTML while communicating with the server.

As the two technologies work with JSON, data flows seamlessly, making it possible to develop fast and debug easily. To make sense of the entire system, you need to understand only one language, i.e., JavaScript and the JSON document structure.


## Use Cases of MERN

Like other popular web stacks, it is possible to develop whatever you want in MERN. Nonetheless, it is ideal for cloud-based projects where you require intensive JSON and dynamic web interfaces. A few examples of purposes where MERN is used are:

**Calendars and To-do Apps**  
A calendar or a to-do app is a rudimentary project that can tell you a lot about the mechanics of the MERN stack. You can design the frontend, i.e., the interface of the calendar or to-do app using ReactJS. The data to be stored, accessed, modified, shown in the to-do app is made possible using MongoDB.

**Interactive Forums**  
Another suitable use case for MERN is an interactive forum, which can be a social media platform or a website that allows users to share messages and communicate. The topic of the interactive forum may or may not be predefined.

**Social Media Product**  
An interactive forum is just one use of the MERN stack for social media. These include ads, posts, a mini web app embedded in the social media page, etc.

---
## Database Management Systems (DBMS)

Check source [here](https://www.techopedia.com/definition/24361/database-management-systems-dbms)

**What is a DBMS?**  
A database management system (DBMS) is middleware that allows programmers, database administrators (DBAs), software applications and end users to store, organize, access, query and manipulate data in a database. 

DBMSs are important because they provide efficient and reliable mechanisms for organizing, managing and using vast amounts of data while also ensuring data integrity and providing other data management benefits. 

In the enterprise, database management systems provide database administrators (DBAs) with a structured framework that facilitates data sharing among different departments, teams and applications. The DBMS provides employees with controlled and organized access to data that they can use to drive innovation and help their company maintain a competitive edge.

**Database vs DBMS**  
The terms “database” and “database management system” are often used interchangeably in casual conversations. That’s probably because when end users interact with a database, they are not aware of the underlying DBMS and its distinct role in managing data. To add to the confusion, in some cases the DBMS is embedded directly into application code. This makes it even less apparent that a separate system is involved.

To differentiate between the two terms and use them correctly, it’s helpful to understand their respective roles and functionalities: A database is a structured collection of data. The database management system is the software that developers, end users and applications use to interact with a database.

![Alt text](Project3_images/dbms.png)

## Types of Database Management Systems

Until the turn of the century, database management systems were classified as either being relational or non-relational, depending on their structure and uses. If the DBMS stored data in tables, it was referred to as a relational DBMS (RDBMS). If it did not store data in tables, it was referred to as a NoSQL or non-relational DBMS.

Today, database management systems are still categorized as being either RDBMS or non-RDBMS, but they are also classified by the unique advantages they provide. Types of DBMSs include:

**Cloud Database Management Systems** – Cloud DBMSs like Amazon Aurora are designed to manage distributed data stored in a cloud provider’s remote data centers. 

**Columnar Database Management Systems** – Columnar DBMSs like Apache Cassandra return queries faster by storing data in columns instead of rows. This schema makes it easier for data analytics and business intelligence applications to work with large datasets.

**Distributed Database Management Systems** – DDBMS functionalities like those found in the Apache Hadoop ecosystem are designed to ensure data integrity for logically-related databases across multiple locations or computing environments. 

**Graph Database Management Systems** – These systems are designed to support graph databases that store relationships at the individual record level. Graph DBMSs like Neo4j are ideal for managing data with interconnected relationships, such as social media data. 

**Hierarchical Database Management Systems** – Hierarchical management systems are designed to support databases organized in parent-child relationships. This type of DBMS has its roots in mainframe computing and its uses today are limited. 

**HTAP Database Management Systems** – Hybrid transaction/analytical processing DBMSs are designed to support mixed workloads for transactional and analytical data. Traditional database systems often have separate systems for online transaction processing (OLTP) and online analytical processing (OLAP) workloads. HTAP management systems like SAP HANA and CockroachDB provide a unified platform that can handle both types of tasks concurrently.

**In-memory Database Management Systems** – In-memory management systems are designed to reduce latency by using main memory for data management and storage. Volt Active Data and other IMDBMSs make data retrieval significantly faster and improve overall system performance.

**Object-oriented database management system** (OODBMS) – db4o is one example of this type of DBMS. OODMBSs are designed to manage complex data structures as storage objects. 

**NewSQL Database Management Systems** — NewSQL DBMSs like PostgreSQL provide the scalability and performance benefits of NoSQL databases while retaining the ACID properties of traditional relational databases. This type of DBMS is designed for large-scale distributed environments and can handle high-throughput transactional workloads.

**Time-Series Database Management Systems** — Time-series DBMSs like InfluxDB optimize the storage, retrieval and analysis of time-stamped data. They are often used to support financial analytics and Internet of Things (IoT) monitoring systems.

## Well-Known Database Management Systems
Examples of well-known DBMSes include: 

&nbsp;  

![Alt text](Project3_images/Access.svg)  
**ACCESS** – a lightweight relational database management system (RDMS) included in Microsoft Office and Office 365.

&nbsp;

![Alt text](Project3_images/Amazon-RDS.svg)  
**Amazon RDS** – a native cloud DBMS that offers engines for managing MySQL, Oracle, SQL Server, PostgreSQL and Amazon Aurora databases.

&nbsp;

![Alt text](Project3_images/cassandra.svg)  
Apache Cassandra – an open-source distributed database management system known for being able to handle massive amounts of data.

&nbsp;

![Alt text](Project3_images/filemaker.svg)  
**Filemaker** – a low-code/no-code (LCNC) relational DBMS.

&nbsp;

![Alt text](Project3_images/Google-Cloud-Spanner.svg)  
**Google Cloud Spanner** — a globally distributed, horizontally scalable, and strongly consistent relational database service offered by Google Cloud.

&nbsp;

![Alt text](Project3_images/ibmdb2.svg)  
**IBM Db2** — a family of relational database management systems developed by IBM that offers various editions for different environments and workloads.

&nbsp;

![Alt text](Project3_images/mariadb.svg)  
**MariaDB** – an open-source relational database fork of MySQL.

&nbsp;

![Alt text](Project3_images/microsoftsqlserver.svg)  
**Microsoft Azure SQL Database** — a cloud-based relational database service provided by Microsoft Azure that offers fully-managed SQL databases.

&nbsp;

![Alt text](Project3_images/mongodb.svg)  
**MongoDB** — A popular NoSQL database management system that uses a document-oriented schema to provide high scalability and flexibility.

&nbsp;

![Alt text](Project3_images/mysql.svg)  
**MySQL** – an open-source relational database management system (RDBMS) owned by Oracle.

&nbsp;

![Alt text](Project3_images/oracle.svg)  
**Oracle** – a proprietary RDMS optimized for hybrid cloud architectures.

&nbsp;

![Alt text](Project3_images/postgresql.svg)  
**PostgreSQL** — an open-source relational database management system known for its robustness, scalability and extensive feature sets.

&nbsp;

![Alt text](Project3_images/sap.svg)  
**SAP HANA** — an in-memory, column-oriented RDBMS optimized for real-time data ingestion and high-performance analytics. 

&nbsp;

![Alt text](Project3_images/sqlazure.svg)  
**SQL Server** – an enterprise-level relational database management system from Microsoft that is capable of handling extremely large volumes of data and database queries.

&nbsp;

![Alt text](Project3_images/sql-lite-1.svg)  
**SQLite** — a lightweight, file-based relational database engine that is widely used in embedded systems and mobile applications.

&nbsp;

![Alt text](Project3_images/teradata.svg)  
**Teradata** – a powerful SQL engine that provides scalable solutions for managing and analyzing large volumes of data.


## Benefits of Using a DBMS

Database management systems DBMSs are especially crucial in situations where multiple users or applications interact with the same databases simultaneously. The DBMS safeguards against conflicts and errors with concurrency control mechanisms that will ensure that even in high-traffic scenarios, data integrity remains intact.

Another benefit is that database management systems offer a wide range of security features, mechanisms and functionalities. Administrators can define access control rules, assign user roles and specify permissions to ensure that only authorized individuals can enter, access and manipulate data. 

Because DBMSs provide audit trails and logging capabilities to track and monitor data access use and modifications, they are useful compliance tools. 

For example, a DBMS can help admins manage data lifecycle management by implementing policies for data retention, archival and eventual disposal. A DBMS can also help enforce privacy controls by providing mechanisms that anonymize or encrypt sensitive data.

## Challenges of Database Management Systems

Although database management systems have revolutionized the way small and large businesses handle and manage data, the learning curve for enterprise DBMS implementation and management can be challenging. This is especially true if the DBMS needs to be integrated with enterprise resource planning (ERP) systems or customer relationship management (CRM) platforms.

Rolling out a new DBMS can also be expensive. Even mid-size businesses will most likely need to hire or contract with a skilled database administrator to ensure their DBMS is properly configured, maintained and optimized. Licensing fees, hardware infrastructure, software upgrades and ongoing maintenance expenses can also strain budgets, especially for smaller organizations.

## Future of the DBMS

Today’s DBMSs are incorporating cutting-edge technologies such as artificial intelligence (AI), machine learning (ML) and blockchain to tackle the challenges of big data, and help organizations stay compliant with relevant regulations and standards for data management.

DBMSs equipped with AI and ML capabilities can automate tasks such as query optimization, data indexing and anomaly detection. Intelligent database management systems can learn from data patterns, adapt to changing workloads and optimize performance autonomously.  

Blockchain-enabled databases can provide immutable, transparent data storage and enable secure, auditable transactions. This type of database management system eliminates the need for central authorities while still enhancing data integrity. It makes them ideal for industries like finance, supply chain and healthcare, where the risks and impacts of data tampering are significant.  

DBMS with built-in stream processing capabilities are becoming vital for use cases like real-time analytics, fraud detection and personalized customer experiences.  With the rise of the Internet of Things (IoT) and streaming data sources, DBMSs will need to handle real-time data processing even more efficiently.

---

## Web frameworks

Check source [here](https://en.wikipedia.org/wiki/Web_framework)

A web framework (WF) or web application framework (WAF) is a software framework that is designed to support the development of web applications including web services, web resources, and web APIs. Web frameworks provide a standard way to build and deploy web applications on the World Wide Web. Web frameworks aim to automate the overhead associated with common activities performed in web development. For example, many web frameworks provide libraries for database access, templating frameworks, and session management, and they often promote code reuse.[1] Although they often target development of dynamic web sites, they are also applicable to static websites.[2]

**History of Web Frameworks**  
As the design of the World Wide Web was not inherently dynamic, early hypertext consisted of hand-coded HTML text files that were published on web servers. Any modifications to published pages needed to be performed by the pages' author. In 1993, the Common Gateway Interface (CGI) standard was introduced for interfacing external applications with web servers, to provide a dynamic web page that reflected user inputs.[3]

Original implementations of the CGI interface typically had adverse effects on the server load however, because each request started a separate process.[4] More recent implementations utilize persistent processes amongst other techniques to reduce the footprint in the server's resources and offer a general performance boost.[citation needed]

In 1995, fully integrated server/language development environments first emerged and new web-specific languages were introduced, such as ColdFusion, PHP, and Active Server Pages.[citation needed]

Although the vast majority of languages for creating dynamic web pages have libraries to help with common tasks, web applications often require specific libraries for particular tasks, such as creating HTML (for example, Jakarta Server Faces).[citation needed]

In the late 1990s, mature, "full stack" frameworks began to appear, that often gathered multiple libraries useful for web development into a single cohesive software stack for web developers to use. Examples of this include ASP.NET, Java EE, WebObjects, web2py, OpenACS, Catalyst, Mojolicious, Ruby on Rails, Laravel, Grails, Django, Zend Framework, Sails.js, Yii,[5] CakePHP,[6] and Symfony.

## Types of framework architectures

Most web frameworks are based on the model–view–controller (MVC) pattern

**Model–view–controller (MVC)**  
Many frameworks follow the MVC architectural pattern to separate the data model into business rules (the "controller") and the user interface (the "view"). This is generally considered a good practice as it modularizes code, promotes code reuse, and allows multiple interfaces to be applied. In web applications, this permits different views to be presented, for example serving different web pages for mobile vs. desktop browsers, or providing machine-readable web service interfaces.

**Push-based vs. pull-based**  
Most MVC frameworks follow a push-based architecture also called "action-based". These frameworks use actions that do the required processing, and then "push" the data to the view layer to render the results.[7] Django, Ruby on Rails, Symfony, Spring MVC, Stripes, Sails.js, CodeIgniter[8] are good examples of this architecture. An alternative to this is pull-based architecture, sometimes also called "component-based". These frameworks start with the view layer, which can then "pull" results from multiple controllers as needed. In this architecture, multiple controllers can be involved with a single view. Lift, Tapestry, JBoss Seam, Jakarta Server Faces, and Wicket are examples of pull-based architectures. Play, Struts, RIFE, and ZK have support for both push- and pull-based application controller calls.

**Three-tier organization**  
In three-tier organization, applications are structured around three physical tiers: client, application, and database.[9][10][11][12] The database is normally an RDBMS. The application contains the business logic, running on a server and communicates with the client using HTTP.[13] The client on web applications is a web browser that runs HTML generated by the application layer.[14][15] The term should not be confused with MVC, where, unlike in three-tier architecture, it is considered a good practice to keep business logic away from the controller, the "middle layer".

## Framework applications

Frameworks are built to support the construction of internet applications based on a single programming language, ranging in focus from general purpose tools such as Zend Framework and Ruby on Rails, which augment the capabilities of a specific language, to native-language programmable packages built around a specific user application, such as content management systems (CMS), some mobile development tools and some portal tools.

**General-purpose website frameworks**  
Web frameworks must function according to the architectural rules of browsers and protocols such as HTTP, which is stateless. Webpages are served up by a server and can then be modified by the browser using JavaScript. Either approach has its advantages and disadvantages.[citation needed]

Server-side page changes typically require that the page be refreshed, but allow any language to be used and more computing power to be utilized. Client-side changes allow the page to be updated in small chunks which feels like a desktop application, but are limited to JavaScript and run in the user's browser, which may have limited computing power. Some mix of the two is typically used.[19] Applications which make heavy use of JavaScript and only refresh parts of the page, are called single-page applications and typically make use of a client-side JavaScript web framework to organize the code.

**Server-side frameworks include:**  
Apache Wicket  
ASP.NET Core  
CakePHP  
Catalyst  
CodeIgniter  
CppCMS  
Django  
Flask  
Jam.py  
Yii  
Laravel  
Mojolicious  
Ruby on Rails  
Sails.js  
Symfony  
Spring MVC  
VIEwoNLY  
Wt (web toolkit)  
Zend Framework

**Client-side frameworks:**  
Backbone.js  
AngularJS  
Angular  
EmberJS  
ReactJS  
jQuery UI  
Svelte  
and Vue.js  

## Framework Features

Frameworks typically set the control flow of a program and allow the user of the framework to "hook into" that flow by exposing various events.[21] This "inversion of control" design pattern is considered to be a defining principle of a framework, and benefits the code by enforcing a common flow for a team which everyone can customize in similar ways.[21] For example, some popular "microframeworks" such as Ruby's Sinatra (which inspired Express.js) allow for "middleware" hooks prior to and after HTTP requests. These middleware functions can be anything, and allow the user to define logging, authentication and session management, and redirecting.

---

## Responsive Web Design with HTML and CSS

While HTML(the Hypertext Markup Language)  is a markup language used to format/structure a web page, CSS is a design language that you use to make your web page look nice and presentable. CSS stands for Cascading Style Sheets, and you use it to improve the appearance of a web page.

Learn more and practice from the source [here](https://www.freecodecamp.org/learn/2022/responsive-web-design/)

---


## Practice basic JavaScript syntax just for fun.

While HTML and CSS control the content and styling of a page, JavaScript is used to make it interactive. In the JavaScript Algorithm and Data Structures Certification, you'll learn the fundamentals of JavaScript including variables, arrays, objects, loops, and functions.

Practice Javascript [here](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/)

---

## What is a REST API?

Learn more from the source [here](https://www.freecodecamp.org/news/what-is-a-rest-api/)

**An API** (short for Application Programming Interface) allows for two or more applications to communicate with one another and send data back and forth.

**APIs** operated based on a standardized set of rules and they're an integral component of modern-day software development.

There are different API styles, and each one has its unique architecture. One of the most common styles is REST.

In this article, you will learn the basics of REST APIs. You will see an overview of what they are and how they work. You will also learn what makes an API RESTful.

Let's get into it!

**What Is A REST API?**  
REST (short for REpresentational State Transfer) is a software architectural style created by computer scientist Roy Fielding in 2000.

With REST APIs, a client requests a resource. Then the server responds to the client with a representation of the current state of that resource and all relevant information about it in a standardized format, such as JSON or XML.

Learn more from the source [here](https://www.freecodecamp.org/news/what-is-a-rest-api/)

---

# Project 3 Task: Deploy a simple To-Do application that creates To-Do lists like this:

![Alt text](Project3_images/mern.gif)

## Initiation - Preparing prerequisites

In order to complete this project you will need an AWS account and a virtual server with Ubuntu Server OS.

If you do not have an AWS account – go back to Project 1 Step 0 to sign in to AWS free tier account and create a new EC2 Instance of t2.micro family with Ubuntu Server 20.04 LTS (HVM) image. Remember, you can have multiple EC2 instances, but make sure you STOP/TERMINATE the ones you are not working with at the moment to save available free hours.

Hint #1: When you create your EC2 Instances, you can add Tag “Name” to it with a value that corresponds to a current project you are working on – it will be reflected in the name of the EC2 Instance. Like this:

![Alt text](Project3_images/EC2_tag.png)

---
# 1st action - Backend Configuration

- **Update ubuntu**  `sudo apt update`

![Alt text](Project3_images/ubuntu%20update.png)

- **Upgrade ubuntu** `sudo apt upgrade`

![Alt text](Project3_images/upgrade%20ubuntu.png)

**Lets get the location of Node.js software from Ubuntu repositories.**

`curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -`

![Alt text](Project3_images/node.png)

**Install Node Js on the server**

`sudo apt-get install -y nodejs`

![Alt text](Project3_images/Screenshot%20at%20Jun%2010%2023-00-06.png)

**Note:** The command above installs both nodejs and npm. NPM is a package manager for Node like apt for Ubuntu, it is used to install Node modules & packages and to manage dependency conflicts.

**Verify the node installation with the command below**

`node -v `

![Alt text](Project3_images/n-version.png)

**Verify the npm installation with the command below**

`npm -v`

![Alt text](Project3_images/npm%20v.png)

**Application code setup**

Create a new directory for your To-Do project:

`mkdir Todo`

Run the command below to verify that the Todo directory is created with ls command

`ls`

![Alt text](Project3_images/mkdir%20todo.png)

**TIP:** In order to see some more useful information about files and directories, you can use following combination of keys ls -lih – it will show you different properties and size in human readable format. You can learn more about different useful keys for ls command with ls --help.

Now change your current directory to the newly created one:

`cd Todo`

Next, you will use the command npm init to initialise your project, so that a new file named package.json will be created. This file will normally contain information about your application and the dependencies that it needs to run. Follow the prompts after running the command. You can press Enter several times to accept default values, then accept to write out the package.json file by typing yes.

`npm init`

![Alt text](Project3_images/npm%20init.png)

**Run the command ls to confirm that you have package.json file created.**

`ls`

![Alt text](Project3_images/p.j.png)

**Next, we will Install ExpressJs and create the Routes directory.**

Remember that Express is a framework for Node.js, therefore a lot of things developers would have programmed is already taken care of out of the box. Therefore it simplifies development, and abstracts a lot of low level details. For example, Express helps to define routes of your application based on HTTP methods and URLs.

**To use express, install it using npm:**

`npm install express`

![Alt text](Project3_images/express%20js.png)

**Now create a file index.js with the command below**

`touch index.js`

**Run `ls` to confirm that your index.js file is successfully created**

![Alt text](Project3_images/Ls-indexjs.png)

**Install the dotenv module**

`npm install dotenv`

![Alt text](Project3_images/dotenv.png)

**Open the index.js file with the command below**

`vim index.js`

**Type the code below into it and save. Do not get overwhelmed by the code you see. For now, simply paste the code into the file.**

```const express = require('express');
require('dotenv').config();

const app = express();

const port = process.env.PORT || 5000;

app.use((req, res, next) => {
res.header("Access-Control-Allow-Origin", "\*");
res.header("Access-Control-Allow-Headers", "Origin, X-Requested-With, Content-Type, Accept");
next();
});

app.use((req, res, next) => {
res.send('Welcome to Express');
});

app.listen(port, () => {
console.log(`Server running on port ${port}`)
});
```

**Notice that we have specified to use port 5000 in the code. This will be required later when we go on the browser.**

Use `:w` to save in vim and use `:qa` to exit vim

**Now it is time to start our server to see if it works. Open your terminal in the same directory as your index.js file and type:**

`node index.js`

If every thing goes well, you should see Server running on port 5000 in your terminal.

![Alt text](Project3_images/serv%20run%205000.png)

Now we need to open this port in EC2 Security Groups. Refer to Project 1 Step 1 – Installing the Nginx Web Server. There we created an inbound rule to open TCP port 80, you need to do the same for port 5000, like this:

![Alt text](Project3_images/Port_5000.png)

**Open up your browser and try to access your server’s Public IP or Public DNS name followed by port 5000:**

`http://<PublicIP-or-PublicDNS>:5000`

`http://34.220.200.255:5000`

Quick reminder how to get your server’s Public IP and public DNS name:
1. You can find it in your AWS web console in EC2 details
2. Run `curl -s http://169.254.169.254/latest/meta-data/public-ipv4` for Public IP address or `curl -s http://169.254.169.254/latest/meta-data/public-hostname` for Public DNS name.


![Alt text](Project3_images/welcome%20to%20Express.png)

**Routes**

There are three actions that our To-Do application needs to be able to do:

1. Create a new task  
2. Display list of all tasks  
3. Delete a completed task  

Each task will be associated with some particular endpoint and will use different standard HTTP request methods: POST, GET, DELETE.

For each task, we need to create routes that will define various endpoints that the To-do app will depend on. So let us create a folder **routes**

`mkdir routes`

**Tip:** You can open multiple shells in Putty or Linux/Mac to connect to the same EC2

**Change directory to routes folder.**

`cd routes`

**Now, create a file api.js with the command below**

`touch api.js`

![Alt text](Project3_images/api%20js.png)

**Open the file with the command below**

`vim api.js`

**Copy below code in the file. (Do not be overwhelmed with the code)**

```
const express = require ('express');
const router = express.Router();

router.get('/todos', (req, res, next) => {

});

router.post('/todos', (req, res, next) => {

});

router.delete('/todos/:id', (req, res, next) => {

})

module.exports = router;
```

Moving forward let create Models directory.

**Models**

Now comes the interesting part, since the app is going to make use of Mongodb which is a NoSQL database, we need to create a model.

A model is at the heart of JavaScript based applications, and it is what makes it interactive.

We will also use models to define the database schema . This is important so that we will be able to define the fields stored in each Mongodb document. (Seems like a lot of information, but not to worry, everything will become clear to you over time. I promise!!!)

In essence, the Schema is a blueprint of how the database will be constructed, including other data fields that may not be required to be stored in the database. These are known as virtual properties

To create a Schema and a model, install mongoose which is a Node.js package that makes working with mongodb easier.

Change directory back Todo folder with `cd ..` and install Mongoose with `npm install mongoose`

![Alt text](Project3_images/mongoose.png)

Create a new folder models:

`mkdir models`

Change directory into the newly created ‘models’ folder with

`cd models`

Inside the models folder, create a file and name it todo.js

`touch todo.js`

Tip: All three commands above can be defined in one line to be executed consequently with help of && operator, like this:

`mkdir models && cd models && touch todo.js`

Open the file created with `vim todo.js` then paste the code below in the file:

```
const mongoose = require('mongoose');
const Schema = mongoose.Schema;

//create schema for todo
const TodoSchema = new Schema({
action: {
type: String,
required: [true, 'The todo text field is required']
}
})

//create model for todo
const Todo = mongoose.model('todo', TodoSchema);

module.exports = Todo;
```

Now we need to update our routes from the file api.js in ‘routes’ directory to make use of the new model.

In Routes directory, open api.js with `vim api.js`, delete the code inside with `:%d` command and paste the code below into it then save and exit

```
const express = require ('express');
const router = express.Router();
const Todo = require('../models/todo');

router.get('/todos', (req, res, next) => {

//this will return all the data, exposing only the id and action field to the client
Todo.find({}, 'action')
.then(data => res.json(data))
.catch(next)
});

router.post('/todos', (req, res, next) => {
if(req.body.action){
Todo.create(req.body)
.then(data => res.json(data))
.catch(next)
}else {
res.json({
error: "The input field is empty"
})
}
});

router.delete('/todos/:id', (req, res, next) => {
Todo.findOneAndDelete({"_id": req.params.id})
.then(data => res.json(data))
.catch(next)
})

module.exports = router;
```

The next piece of our application will be the MongoDB Database

**MongoDB Database**

We need a database where we will store our data. For this we will make use of mLab. mLab provides MongoDB database as a service solution (DBaaS), so to make life easy, you will need to sign up for a shared clusters free account, which is ideal for our use case. Sign up here. Follow the sign up process, select AWS as the cloud provider, and choose a region near you.

Complete a get started checklist as shown on the image below

![Alt text](Project3_images/Create-a-Cluster.png)

![Alt text](Project3_images/ceration-of-username-and-password.png)

Allow access to the MongoDB database from anywhere (Not secure, but it is ideal for testing)

IMPORTANT NOTE
In the image below, make sure you change the time of deleting the entry from 6 Hours to 1 Week

![Alt text](Project3_images/MogoDB-Network-Access.png)

![Alt text](Project3_images/Browse-Collections.png)

![Alt text](Project3_images/From%20coll%20to%20overview%20tab.png)

In the **index.js** file, we specified **process.env** to access environment variables, but we have not yet created this file. So we need to do that now.

Create a file in your Todo directory and name it .env.

```
touch .env
```

Follow image examples below to get the connection string and save in a format like this: `DB=mongodb+srv://<username>:<password>@<network-address>/<dbname>?retryWrites=true&w=majority` to access the MongoDB database. 


**Here is how to get your connection string**

![Alt text](Project3_images/connect-to-cluster.png)

![Alt text](Project3_images/click-on-mongodb-driver.png)

![Alt text](Project3_images/connect-to-cluster1.png)


Ensure to update the username, password, network-address, and database name according to your setup. In most cases only password and database name requires update. format like this: `DB=mongodb+srv://<username>:<password>@<network-address>/<dbname>?retryWrites=true&w=majority`(example: DB=mongodb+srv://username:password@project3-dbcluster.vrzzagv.mongodb.net/Project3-DBcluster
?retryWrites=true&w=majority)

While in **Todo directory**, use `vi .env` command to open .env file, copy the connection string, paste it into the vi editor. Use command `:wq` to save and quit the vi editor.




Now we need to update the **index.js** to reflect the use of **.env** so that **Node.js** can connect to the database.

Simply delete existing content in the file, and update it with the entire code below.



To do that using vim, follow below steps

1. Open the file with `vim index.js`
2. Press `esc`
3. Type :%d
4. Hit ‘Enter’

The entire content will be deleted, then,

5. Press `i` to enter the insert mode in vim
6. Now, paste the entire code below in the file.

```
const express = require('express');
const bodyParser = require('body-parser');
const mongoose = require('mongoose');
const routes = require('./routes/api');
const path = require('path');
require('dotenv').config();

const app = express();

const port = process.env.PORT || 5000;

//connect to the database
mongoose.connect(process.env.DB, { useNewUrlParser: true, useUnifiedTopology: true })
.then(() => console.log(`Database connected successfully`))
.catch(err => console.log(err));

//since mongoose promise is depreciated, we overide it with node's promise
mongoose.Promise = global.Promise;

app.use((req, res, next) => {
res.header("Access-Control-Allow-Origin", "\*");
res.header("Access-Control-Allow-Headers", "Origin, X-Requested-With, Content-Type, Accept");
next();
});

app.use(bodyParser.json());

app.use('/api', routes);

app.use((err, req, res, next) => {
console.log(err);
next();
});

app.listen(port, () => {
console.log(`Server running on port ${port}`)
});

```

Using environment variables to store information is considered more secure and best practice to separate configuration and secret data from the application, instead of writing connection strings directly inside the index.js application file.

Start your server using the command:

`node index.js`

You shall see a message ‘Database connected successfully’

![Alt text](Project3_images/DB%20connection%20successful.png)

We have our backend configured. Now we are going to test it.

## Testing Backend Code without Frontend using RESTful API

So far we have written backend part of our To-Do application, and configured a database, but we do not have a frontend UI yet. We need ReactJS code to achieve that. But during development, we will need a way to test our code using RESTfull API. Therefore, we will need to make use of some API development client to test our code.

In this project, we will use [Postman](https://www.postman.com/) to test our API.
Click [Install Postman](https://www.postman.com/downloads/) to download and install postman on your machine.

Click [HERE](https://www.youtube.com/watch?v=FjgYtQK_zLE) to learn how to perform [CRUD operations](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete) on Postman

You should test all the API endpoints and make sure they are working. For the endpoints that require body, you should send JSON back with the necessary fields since it’s what we setup in our code.

Now open your Postman, create a POST request to the API http://<PublicIP-or-PublicDNS>:5000/api/todos. This request sends a new task to our To-Do list so the application could store it in the database.

**Note:** make sure you set header key Content-Type as application/json

![Alt text](Project3_images/postman_header.png)

Check the image below:

![Alt text](Project3_images/post-request.jpeg)

Create a GET request to your API on http://<PublicIP-or-PublicDNS>:5000/api/todos. This request retrieves all existing records from our To-do application (backend requests these records from the database and sends it back to us as a response to GET request).

![Alt text](Project3_images/get-request.jpeg)

**Optional task:** Try to figure out how to send a DELETE request to delete a task from our To-Do list.

**Hint:** To delete a task – you need to send its ID as a part of DELETE request.

By now you have tested backend part of our To-Do application and have made sure that it supports all three operations we wanted:

- [x] Display a list of tasks – HTTP GET request
- [x] Add a new task to the list – HTTP POST request
- [x] Delete an existing task from the list – HTTP DELETE request

We have successfully created our Backend, now let go create the Frontend.

---

# 2nd action - Frontend Creation

Since we are done with the functionality we want from our backend and API, it is time to create a user interface for a Web client (browser) to interact with the application via API. To start out with the frontend of the To-do app, we will use the `create-react-app` command to scaffold our app.

In the same root directory as your backend code, which is the **Todo** directory, run:

```
npx create-react-app client
```

This will create a new folder in your Todo directory called client, where you will add all the react code.

install successfullyl, see image below

![Alt text](Project3_images/reactjs%20client.png)

## **Running a React App:**

Before testing the react app, there are some dependencies that need to be installed.

1. Install concurrently. It is used to run more than one command simultaneously from the same terminal window.

```
npm install concurrently --save-dev
```

installed, see below

![Alt text](Project3_images/intalled%20conc.png)

2. Install nodemon. It is used to run and monitor the server. If there is any change in the server code, nodemon will restart it automatically and load the new changes.

```
npm install nodemon --save-dev
```
installed, see below

![Alt text](Project3_images/inst%20nodemon.png)

3. In Todo folder open the package.json file. Change the highlighted part of the below screenshot and replace with the code below.

```
"scripts": {
"start": "node index.js",
"start-watch": "nodemon index.js",
"dev": "concurrently \"npm run start-watch\" \"cd client && npm start\""
},
```
Edited sample below

![Alt text](Project3_images/package%20json.png)

## Configure Proxy in package.json

1. Change directory to ‘client’

```
cd client
```
2. Open the package.json file

```
vi package.jason
```

3. Add the key value pair in the package.json file `"proxy": "http://localhost:5000"`

The whole purpose of adding the proxy configuration in number 3 above is to make it possible to access the application directly from the browser by simply calling the server url like http://localhost:5000 rather than always including the entire path like http://localhost:5000/api/todos

Now, ensure you are inside the Todo directory, and simply do:

```
npm run dev
```

Your app should open and start running on localhost:3000

**Important note:** In order to be able to access the application from the Internet you have to open TCP port 3000 on EC2 by adding a new Security Group rule. You already know how to do it.

Creating your React Components
One of the advantages of react is that it makes use of components, which are reusable and also makes code modular. For our Todo app, there will be two stateful components and one stateless component.
From your Todo directory run

```
cd client
```

move to the src directory

```
cd src
```
Inside your src folder create another folder called components

```
mkdir components
```
Move into the components directory with

```
cd components
```
Inside ‘components’ directory create three files **Input.js**, **ListTodo.js** and **Todo.js**.

```
touch Input.js ListTodo.js Todo.js
```
Open Input.js file

```
vi Input.js
```

Copy and paste the following

```
import React, { Component } from 'react';
import axios from 'axios';

class Input extends Component {

state = {
action: ""
}

addTodo = () => {
const task = {action: this.state.action}

    if(task.action && task.action.length > 0){
      axios.post('/api/todos', task)
        .then(res => {
          if(res.data){
            this.props.getTodos();
            this.setState({action: ""})
          }
        })
        .catch(err => console.log(err))
    }else {
      console.log('input field required')
    }

}

handleChange = (e) => {
this.setState({
action: e.target.value
})
}

render() {
let { action } = this.state;
return (
<div>
<input type="text" onChange={this.handleChange} value={action} />
<button onClick={this.addTodo}>add todo</button>
</div>
)
}
}

export default Input
```

To make use of Axios, which is a Promise based HTTP client for the browser and node.js, you need to cd into your client from your terminal and run yarn add axios or npm install axios.

Move to the src folder

```
cd ..
```
Move to clients folder

```
cd ..
```
Install Axios

```
npm install axios
```
Sip a coffee, click on the next button and let finish this up.

























