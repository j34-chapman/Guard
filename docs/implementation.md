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

Views was the third folder and contained all of the embedded javascript templates (ejs files) which allowed for dynamic content to be utilised by the project. head.ejs contained the links to the style.css file and stylesheets which allows for all files with the head file including within to utilise these other files. header.ejs contained the title of the project and its corresponding style which would span across the top of all pages of which is was included within. index.ejs was the splash page which was loaded upon loading of the website and contains a map of the data provided by opendata bristol. nav.ejs and nav2.ejs both provided similar functions of having the buttons to navigate the website, with nav2.ejs also including a search bar for when no longer located on the home page (index.ejs). These buttons lead to the following files. fsa.ejs , which provided access to a table containing use case 1, the dataset sorted by crime numbers in ascending order. viewbycategory.ejs provides buttons to the webpage to allow


## Software Architecture
TODO: Describe the major components of your architecture. Are any particular architectural styles being used?

![Software Architecture diagram Implmentation](https://user-images.githubusercontent.com/93520494/143852891-3ae9cd20-afef-48d6-93e9-b9d3387cb71e.png)
