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
TODO: Describe each use case (one per team member).
    Give each use case a unique ID, e.g. UC1, UC2, ...
    Summarise these using the use-case template below.

| TODO: USE-CASE ID e.g. UC1, UC2, ... | TODO: USE-CASE NAME | 
| -------------------------------------- | ------------------- |
| **UC1** | Searching for a preferred safe route home |
| **Actors** | Pedestrian |
| **Assumptions** | Pre-conditions: Log in to the application > Enter desired destination address > Select route based on rate of  crime in different areas. Post-conditions: Select a different route based on rate of crime in different area
| **Steps** | 1. *Opt to view map and different routes to selected destination address* 2. Request Permission to access user location 3. *Give Permission for geo-location (on request)* 4. Get fastest route to destination address and display areas exhibiting crime rates 5. *View map navigator towards destination address* |
| **Variations** | Allow application to select recommended route based of safest route (walking through the lowest crime rate path). |
| **Non-functional** | The service should run on different web browsers (Microsoft Edge, Google Chrome, Internet Explorer) |
| **Issues** | N/A |

| TODO: USE-CASE ID e.g. UC1, UC2, ... | TODO: USE-CASE NAME | 
| -------------------------------------- | ------------------- |
| **UC2** | Track and Report Crimes |
| **Actors** | Pedestrian, Developer, Emergency Service |
| **Assumptions** |  Pre-conditions: Log in to the application > Select area on the map > Select option to report crime > Enter detailed report/media attatchments > Submit report. Post-conditions: Developers review the report > Emergency Services review the report > Data is shared with BristolOpenData > Crime report is added onto map navigator
| **Steps** | 1. *Opt to view map 2. Opt to select location on map* 3. Display option to report a crime 4. *Opt to report a crime* 5. Display text box and option to add media attachments 6. *Submit detailed report of crime about said area* |
| **Variations** | N/A |
| **Non-functional** | The service should run on different web browsers (Microsoft Edge, Google Chrome, Internet Explorer) |
| **Issues** | N/A |

| TODO: USE-CASE ID e.g. UC1, UC2, ... | TODO: USE-CASE NAME | 
| -------------------------------------- | ------------------- |
| **UC3** | Accessible Emergency Contact |
| **Actors** | Pedestrian, Emergency Service |
| **Assumptions** |  Post-conditions: 
| **Steps** | 1. *Opt to view map 2. Opt to select location on map* 3. Display option to report a crime 4. *Opt to report a crime* 5. Display text box and option to add media attachments 6. *Submit detailed report of crime about said area* |
| **Variations** | N/A |
| **Non-functional** | The service should run on different web browsers (Microsoft Edge, Google Chrome, Internet Explorer) |
| **Issues** | N/A |

TODO: Your Use-Case diagram should include all use-cases.


![UseCase DiagramUpdated](https://user-images.githubusercontent.com/93520494/142854598-5aa67f6b-c627-46f6-9dd8-b2fef9871848.png)

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
