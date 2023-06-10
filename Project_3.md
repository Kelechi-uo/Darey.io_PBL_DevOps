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


## 1st action - Backend Configuration

- **Update ubuntu** 
`sudo apt update`
