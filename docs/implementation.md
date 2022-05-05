# Implementation

## Introduction

The system that we implemented is built through the use of several core components, with these being opendata bristol, sql, npm and express. Opendata bristol provided the dataset which was crime throughout bristol over the span of the past few years. Within this dataset was multiple sections with a large amount of data which was imported into a table within sql, which held the database and linked to the server. This was achieved through the use of a configuration file to allow for easy access to the database seperate to the system. npm was utilised to introduce the express framework which allowed for building the web server with ease.

## Project Structure

At the root of the project are 3 main folders and 2 files. The folders are node_modules, static and views whilst the files are conf.json and main.js

![Project Structure](https://user-images.githubusercontent.com/94834832/166718010-a5f36e87-54cb-476f-900f-aeedef6cb3a1.JPG)

Also present within the folder is a node file, containing binary data of a library of functions for node.js applications and two similar files, package.json and package-lock.json. The role of these files is to contain metadata about the project, such as the dependencies and version. Package-lock.json makes sure the version of all installed packages are kept up to date.

Node_modules, was installed along with npm and express when initialising the project. 

Static, which contains files which are sent to the browser when they are requested. In the case of our project the folder contained the style.css file, which contained the templates to specify the layout of webpages, for example the font and colours of the buttons used throughout different pages.

Views was the third folder and contained all of the embedded javascript templates (ejs files) which allowed for dynamic content to be utilised by the project. head.ejs contained the links to the style.css file and stylesheets which allows for all files with the head file including within to utilise these other files. header.ejs contained the title of the project and its corresponding style which would span across the top of all pages of which is was included within. index.ejs was the splash page which was loaded upon loading of the website and contains a map of the data provided by opendata bristol. nav.ejs and nav2.ejs both provided similar functions of having the buttons to navigate the website, with nav2.ejs also including a search bar for when no longer located on the home page (index.ejs). These buttons lead to the following files. fsa.ejs , which provided access to a table containing use case 1, the dataset sorted by crime numbers in ascending order. Viewbycategory.ejs provides buttons to the webpage to allow for the user to sort the dataset in the table by date or location, whilst providing the unsorted table to the user to view. 
The sort by date button leads to the viewbydate.ejs file which again provides buttons to allow for individual dates to be selected and sorts the table to show only these dates to the user. The sort by location button leads to the viewbyward.ejs file which provides the user with a search bar to allow for locations to be searched.
This search bar leads to the file searchbylocation.ejs which takes in the query from the previous pages search bar and sorts the dataset according to the query passed in.

The two files within the root directory of the project are most importantly the main.js, and the conf.json. the main.js file contains the main code that provides the structure for the web server to run and function, utilising the express framework. The file contains functions to allow for navigating between the different webpages and taking in the different queries needed for sorting the dataset within the tables. A connection to mySQL is also set up within the main.js allowing for the server to actually acess the database. The use of the conf.json file allowed for the connection to the database to be simplified storing the configuration data of the database connection within allowing for simplified access.

### ESlint
Seen below are the results after running ESlint on the main.js of the project:
![eslint](https://user-images.githubusercontent.com/94834832/166737609-952f65ab-7099-44b5-ad69-93a136dd80f4.JPG)

The first three errors are in relation to the first three lines of code within the file. The purpose of these lines of code is to create constant variables of which have access to frameworks installed outside of the main.js file located within the node_modules folder and the config file allowing access to there utility within the project. The error associated with these does not stop the code from working but is due to require not being a valid function within the client-side javascript, however this reference error does not stop the function from loading the external modules.

The other list of errors are due to a variable located within the callback functions for the webpages which load the table of data from mySQL. The fields variable is defined but is never used within the ejs files, due to its functionality not required. However leaving the variables whilst it may negligbly increase the overall size of the project, it also allows for future versions to utilise the variables to manipulate specific fields of data potentially.

## Software Architecture

![Software Architecture diagram Implmentation](https://user-images.githubusercontent.com/93520494/143852891-3ae9cd20-afef-48d6-93e9-b9d3387cb71e.png)

There are three distinct components of the architecture used within our project. These are the guard client, guard server and the database. These three components make up a 3-tier architectural design allowing for inter-process communication between the components The guard client is what the user interacts with and contains the user interface within the application itself and is depended upon the guard server to function. The guard server handles the passing of information to the client and queries to the database allowing for an exchange of data between the components. The server also holds all the relevant information needed to build the webpages within the client, for example the stylesheet data (css file). The guard server is also dependent upon the database, which holds the dataset which is obtained through queries sent through the webserver. The database communicates with the web server to send the data needed depending on the query exchanged between the two components.

