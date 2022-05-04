# Implementation

## Introduction
TODO: Describe the system implemented (Describe the dataset. Are there any known issues? Describe any configuration data).

The system that we implemented is built through the use of several core components, with these being opendata bristol, sql, npm and express. Opendata bristol provided the dataset which was crime throughout bristol over the span of the past few years. Within this dataset was multiple sections with a large amount of data which was imported into a table within sql, which held the database and linked to the server. This was achieved through the use of a configuration file to allow for easy access to the database seperate to the system. npm was utilised to introduce the express framework which allowed for building the web server with ease.

## Project Structure
TODO: Provide an outline of the project folder structure and the role of each file within it (not the contents of node_modules).
provide a table listing the number of jslint warnings/reports for each module.

At the root of the project are 3 main folders and 2 files. The folders are node_modules, static and views whilst the files are conf.json and main.js

Node_modules, was installed along with npm and express when initialising the project. 

Static, which contains files which are sent to the browser when they are requested. In the case of our project the folder contained the style.css file, which contained the templates to specify the layout of webpages, for example the font and colours of the buttons used throughout different pages.

Views was the third folder and contained all of the embedded javascript templates (ejs files) which allowed for dynamic content to be utilised by the project. head.ejs contained the links to the style.css file and stylesheets which allows for all files with the head file including within to utilise these other files. header.ejs contained the title of the project and its corresponding style which would span across the top of all pages of which is was included within. index.ejs was the splash page which was loaded upon loading of the website and contains a map of the data provided by opendata bristol. nav.ejs and nav2.ejs both provided similar functions of having the buttons to navigate the website, with nav2.ejs also including a search bar for when no longer located on the home page (index.ejs). These buttons lead to the following files. fsa.ejs , which provided access to a table containing use case 1, the dataset sorted by crime numbers in ascending order. Viewbycategory.ejs provides buttons to the webpage to allow for the user to sort the dataset in the table by date or location, whilst providing the unsorted table to the user to view. 
The sort by date button leads to the viewbydate.ejs file which again provides buttons to allow for individual dates to be selected and sorts the table to show only these dates to the user. The sort by location button leads to the viewbyward.ejs file which provides the user with a search bar to allow for locations to be searched.
This search bar leads to the file searchbylocation.ejs which takes in the query from the previous pages search bar and sorts the dataset according to the query passed in.

The two files within the root directory of the project are most importantly the main.js, and the conf.json. the main.js file contains the main code that provides the structure for the web server to run and function, utilising the express framework. The file contains functions to allow for navigating between the different webpages and taking in the different queries needed for sorting the dataset within the tables. A connection to mySQL is also set up within the main.js allowing for the server to actually acess the database. The use of the conf.json file allowed for the connection to the database to be simplified storing the configuration data of the database connection within allowing for simplified access.

## Software Architecture
TODO: Describe the major components of your architecture. Are any particular architectural styles being used?

![Software Architecture diagram Implmentation](https://user-images.githubusercontent.com/93520494/143852891-3ae9cd20-afef-48d6-93e9-b9d3387cb71e.png)
