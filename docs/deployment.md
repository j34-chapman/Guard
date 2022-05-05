# Deployment

## Release Notes

### Guard
Current Version: v1.0.0

The current version of Guard is the first release v1.0.0 and has been developed with software tools such as Visual studio code to write the Javascript and ejs files. these files are linked to a database within mySQL. to create this link certain frameworks are required through the use of Node to allow for the installation of the express framework and dependencies for express and mySQL. dependencies for ESlint were also used to allow for better quality of code during the implementation phase of the project. Heroku was used as the deployment platform at the release of the project.
TEST SOFTWARE

Seen below is a UML diagram of the deployment:

![DEPLOYMENT D](https://user-images.githubusercontent.com/94834832/166846443-538f40d9-6efd-4cc2-9c06-efbcadf4ac66.JPG)

Four major components made up the deployment of the project, these being express, ejs, mySQL and the webserver itself. The webserver is dependent upon all of the other components to allow for it to function correctly, with these allowing access to frameworks and libraries within the webserver to create the project. Express and EJS could be found within the Heroku Node. Heroku allowed for a platform of which to deploy the project. The mySQL is not found within this node due to its databases being stored within its own application and not within the project files, however the webserver was still dependent upon this component. The guard client is not found within this node but is dependent on the components within for the application to be deployed and run successfully.  

# User guide
Explanations of each use case along with step-by-step instructions can be found below: 

## Use Case 1
Seen below is the step-by-step guide to using the find safest area feature of the project:

![HOMEPAGE](https://user-images.githubusercontent.com/94834832/166847837-fb1760c4-3b2b-4f43-8e73-020464bddd43.JPG)
1. Starting from the home page of the website, seen on the navigation bar across the header is a button to find the safest area. Selection of this button will take the user to the find safest area webpage as seen next.

![fsa](https://user-images.githubusercontent.com/94834832/166847840-5bc0f3e5-944c-46d7-a360-ca3fe156a33f.JPG)
2. As seen above, a table is loaded which automatically has the query for the lowest crime area. What this does is presents the user with all the data within the table sorted by the lowest crime in ascending order and is displayed within the webpage to the user.

## Use Case 2
Seen below is the step-by-step guide to using the view crime by category feature of the project:

![HOMEPAGE](https://user-images.githubusercontent.com/94834832/166837788-26028f4c-ac08-416e-a13d-c9c4c0629954.JPG)
1. Starting from the home page of the website, seen clearly on the navigation bar across the screen is the option to view the crime data by category. Selection of this option will take the user to the following page.


![viewbycategory](https://user-images.githubusercontent.com/94834832/166837792-a65ba248-0be2-415e-8298-95cff6a50a01.JPG)
2. The user is now presenting with two new points of interest, the table containing all of the unsorted crime data and a second navigation bar with three options. The first option will allow the user to sort the data by the date of which it was obtained, the second option will allow the user to sort the data by its location and the third option allows for the return to the home page.


![viewbydate](https://user-images.githubusercontent.com/94834832/166837794-0a3b3d35-601b-46e4-951b-a03e201cd95c.JPG)
3. If the user opts to select the view by date option on the previous page, they will now be presented with the choice of selecting any of the available time periods of which to sort the data by. as seen in the example above, the table has been sorted by the option of 2020/2021, so that is the only available data within the table to be viewed.


![viewby location](https://user-images.githubusercontent.com/94834832/166837796-af784d42-d7f0-4142-be12-7559d93fbd63.JPG)
4. If the user instead selects the view by location option instead, they will still be presented with an unsorted table however the second navigation bar will have a search bar present, of which the user can enter any queries relevant to a location. pressing the search button will lead to the next webpage.


![searchbylocation](https://user-images.githubusercontent.com/94834832/166837797-bb11c1a4-18b5-430a-bbd4-c86612464037.JPG)
5. With the query entered from the last page's search bar, the unsorted table will now be sorted relative to terms similar to the query entered. In the example above Hengrove was entered into the search bar, and so the table was sorted to show these results.

## Use Case 3
Seen below is the step-by-step guide to using the search bar feature of the project:

![HOMEPAGE](https://user-images.githubusercontent.com/94834832/166847886-34672152-6920-4012-9599-90dbd08a5f03.JPG)
1. From the home page as seen above there is two options available and pressing either of these will lead to webpages where the search bar is available to be interacted with as seen on the following page.

![fsa - search (uc3)](https://user-images.githubusercontent.com/94834832/166847888-3a59d0d7-d937-4bd5-96b8-12ccadc3c4c6.JPG)
2. With one of the two options selected, in this example the find safest area webpage, the search bar will appear at the top right of the navigation bar within the header of the page. From here the user can enter any search terms, in this example the term "Southmead" was used and to execute the search the user must press the search button.

![search uc3](https://user-images.githubusercontent.com/94834832/166847889-6312d986-3f63-4b93-a76d-e6d695898138.JPG)
3. With the search button pressed, the results of the search will be displayed within a table across the webpage. As seen in this example all terms similar to "Southmead" are found and sorted to display.


