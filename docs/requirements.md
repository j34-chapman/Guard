# Requirements

## User Needs

### User stories
TODO: Write brief user stories to explain how various actors would interact with the system to accomplish a goal.
    Express these in the form from agile development:- As a (role) I want (goal) so that (benefit).
    
- As a civilian/pedestrian, I want to find the safest route so I can get home safely
- As a civilian/pedestrian, I want to easily report a crime so that I can feel safe knowing that the information will be used by the Emergency Services and other people
- As a parent, I want to see that my child is arriving to their location safely and be able to see their location incase of an emergency. I will then worry less
- As a policeman, I want to be able to track and monitor crimes in different areas of Bristol, this will help us make potential arrests and send staff to areas to patrol
   

### Actors
TODO: List and describe the actors/users for this product.

- Women
- Men
- Parent
- Child
- Friend
- Family member
- Student
- Worker
- Policeman/Policewoman

### Use Cases


| UC1 | Find Safest Area | 
| -------------------------------------- | ------------------- |
| **UC1** | Find Safest Area |
| **Actors** | Pedestrian |
| **Assumptions** | Pre-conditions: Log in to the application > Select Option/Button to view Safest Area > Select route based on rate of crime in different areas. Post-conditions: Choose safest area to walk in 
| **Steps** |<pre> 1. Opt to view data on safest areas&#13; 2. Display lowest number of crime in ascending order</pre> |
| **Variations** | Find lowest crime per category not just 'Total Crime'. |
| **Non-functional** | The service should run on different web browsers (Microsoft Edge, Google Chrome, Internet Explorer) |
| **Issues** | N/A |

| UC2 | View crime data by category | 
| -------------------------------------- | ------------------- |
| **UC2** | View crime data by category |
| **Actors** | Pedestrian |
| **Assumptions** |  Pre-conditions: Log in to the application > Select option to view data by category > Select category to sort data by > select subcategory to view data Post-conditions: Sort data by selected conditions
| **Steps** |<pre> 1. Opt to view data by category&#13; 2. Opt to select sort by location or date of crime&#13; 3. Display option to select all datas or locations available&#13; 4. Display table of data with conditions selected&#13; 5. Change data in table according to any changes to conditions selected</pre> |
| **Variations** | allow for indivdual years to be selected when sorting by date |
| **Non-functional** | The service should run on different web browsers (Microsoft Edge, Google Chrome, Internet Explorer) |
| **Issues** | N/A |

| UC3 | Search bar for all queries | 
| -------------------------------------- | ------------------- |
| **UC3** | Search bar for all queries  |
| **Actors** | Pedestrians |
| **Assumptions** |  Pre-conditions: Log in to the application > Enter query to be searched into bar located at top right of screen > click button to execute search Post-conditions: search for terms within table using entered query
| **Steps** | <pre> 1. Opt to select search bar at top right&#13; 2. Opt to enter query wished to be searched&#13; 3. Display table with any contents similar to query entered within search bar </pre>  |
| **Variations** | N/A |
| **Non-functional** | The service should run on different web browsers (Microsoft Edge, Google Chrome, Internet Explorer)  |
| **Issues** | N/A |

TODO: Your Use-Case diagram should include all use-cases.

![Updated USE CASE](https://user-images.githubusercontent.com/93520494/166518607-87068fe1-90af-4658-923c-5a2554591203.jpg)




## Software Requirements Specification
### Functional requirements
**FR1:** The system shall get user geo-location from navigator.geolocation

**FR2:** The system shall display crime rates in different areas surround the path towards destination address from database


### Non-Functional Requirements
NFR1: It should authenticate each user on the app with an id application (Fucntionality (Security))

NFR2: User data should not be disributed or acessbile by others (Functionality (Safety))

NFR3: It should link a reporting to someones to account Data (Functionality (Tracability))

NFR4: Manipulation of data must be reported (Functionality (Accountablity))

TODO: Consider one or more [quality attributes](https://en.wikipedia.org/wiki/ISO/IEC_9126) to suggest a small number of non-functional requirements.
Give each non-functional requirement a unique ID. e.g. NFR1, NFR2, ...

Indicate which UC the requirement comes from.
