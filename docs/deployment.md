# Deployment

## Release Notes
TODO: Describe the current version of the system (with version number. Include system dependencies ands software tools used.
Are there any known issues? 

Describe the deployment of software components to hardware nodes using a UML Deployment diagram.

### Guard
Current Version: v1.0.0

The current version of Guard is the first release v1.0.0 and has been developed with software tools such as Visual studio code to write the Javascript and ejs files. these files are linked to a database within mySQL. to create this link certain frameworks are required through the use of Node to allow for the installation of the express framework and dependencies for express and mySQL. dependencies for ESlint were also used to allow for better quality of code


Seen below is a UML diagram of the deployment:

![WEB](https://user-images.githubusercontent.com/93520494/165071233-0a9447ab-d547-4c07-87fa-e47d6b7cbd12.png)

Four major components made up the deployment of the project, these being express, ejs, mySQL and the webserver itself. The webserver is dependent upon all of the other components to allow for it to function correctly, with these allowing access to frameworks and libraries within the webserver to create the project. 

# User guide
Explanations of each use case along with step-by-step instructions can be found below: 

## Use Case 1

## Use Case 2
Seen below is the step-by-step guide to using the view crime by category feature of the project:

![HOMEPAGE](https://user-images.githubusercontent.com/94834832/166837788-26028f4c-ac08-416e-a13d-c9c4c0629954.JPG)
1) Starting from the home page of the website, seen clearly on the navigation bar across the screen is the option to view the crime data by category. selection of this option will take the user to the following page.


![viewbycategory](https://user-images.githubusercontent.com/94834832/166837792-a65ba248-0be2-415e-8298-95cff6a50a01.JPG)
2) The user is now presenting with two new points of interest, the table containing all of the unsorted crime data and a second navigation bar with three options. The first option will allow the user to sort the data by the date of which it was obtained, the second option will allow the user to sort the data by its location and the third option allows for the return to the home page.


![viewbydate](https://user-images.githubusercontent.com/94834832/166837794-0a3b3d35-601b-46e4-951b-a03e201cd95c.JPG)
3) If the user opts to select the view by date option on the previous page, they will now be presented with the choice of selecting any of the available time periods of which to sort the data by. as seen in the example above, the table has been sorted by the option of 2020/2021, so that is the only available data within the table to be viewed.


![viewby location](https://user-images.githubusercontent.com/94834832/166837796-af784d42-d7f0-4142-be12-7559d93fbd63.JPG)
4) If the user instead selects the view by location option instead, they will still be presented with an unsorted table however the second navigation bar will have a search bar present, of which the user can enter any queries relevant to a location. pressing the search button will lead to the next webpage.


![searchbylocation](https://user-images.githubusercontent.com/94834832/166837797-bb11c1a4-18b5-430a-bbd4-c86612464037.JPG)
5) With the query entered from the last page's search bar, the unsorted table will now be sorted relative to terms similar to the query entered. In the example above Hengrove was entered into the search bar, and so the table was sorted to show these results.

## Use Case 3



TODO: Repeat as necessary
