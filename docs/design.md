# Design

## Behavioural design

![UC1 Sequence Diagram](https://user-images.githubusercontent.com/93520494/166558015-6288e680-2808-4ca5-9f46-cf0bf7584680.jpg)
### UC1 Sequence Diagram Description

![UCSD](https://user-images.githubusercontent.com/94834832/166817373-53faf2f3-bf73-42cc-a7c3-966363e34c14.JPG)

### UC2 Sequence Diagram Description

- Citizen selects view by category

- Categories to select are returned to the display

- Citizen selects the category that they wish to view

- Request is sent to the guard server to get selected category

- This request is sent as a query to the database

- Query is returned to guard server where it is displayed to the guard client as a results table

![UC3 Sequence Diagram](https://user-images.githubusercontent.com/93520494/166569392-19ef49a7-3fcc-4f1f-a9e4-262882a27276.jpg)

### UC3 Sequence Diagram Description

- Citizen clicks on search bar

- Citizen wants to find specific areas crime rate

- Citzen types area of there choice 

- This request then goes to the guard server

- The query is then processed finding all information of "Area.."

- The guard server then returns a results table to Guard with matching Search query


## User Interface design
Below are wireframe prototypes for each of the use cases within the project, along with a description of the proposed layout: 

### Whimsical Wireframe - Airen (UC1)

![26caf472-fdaa-495a-8703-43707a25d620](https://user-images.githubusercontent.com/86235504/148756418-0f5065d2-cde8-415f-8d78-bdbc593b3915.png)

### Whimsical Wireframe - Joe (UC2)

![Wireframe](https://user-images.githubusercontent.com/94834832/166563372-dcd14791-208a-49ce-96a2-ab7902ba8931.png)

Key parts of the website design are as follows:

Within the header of the webpage will be a banner with buttons leading to the corresponding utilities such as pictured above. also present in the header is the search bar allowing access to any queries the user may opt to view.

A home page button which will lead to the main page for the user to access all aspects of the website.

Search safest route button will allow the user to view the safest area in ascending order.

View crime by category button will allow the user to access a new page of the website as seen above. From this page there is two new buttons present on a bar beneath the header - view by date and view by location.

The view by date button allows for access to the same bar beneath the header, however now the options for selecting the different dates are present on the bar as buttons. These buttons will grant access to a sorted table corresponding to the respective date.

The view by location button allows for access to the same bar again however there is now a search bar present with the function of searching any queries for similarities to locations within the table. these will then be sorted and displayed to the user upon pressing of the search button.

### Whimsical Wireframe - Jake (UC3)

![untitled@2x](https://user-images.githubusercontent.com/93520494/164234872-77721d8c-35c7-4a2f-bb10-4e11cd8fddcc.png)

Home Page - Displays the information and function of the website . 

Find Safest Area (Button) - By pressing this will display information of the safest area in ascending order from safest to least safest. 

Find Safest Area (Page - Search Bar) - By searching with this search this will display the given area with the statistics of crime 

Report A Crime - This will load a map displaying the area of the crimes . Then will grant youre user loacation to report the crime.
