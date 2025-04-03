# Requirements

## User Needs

### User stories
User Story: As an EV user, I want to find the nearest charging point that is full so that I can save energy by avoiding unnecessary travel to empty charging points and ensure I can recharge my vehicle efficiently.
 As the council, I want to check all charging points on the app to gather data so that I can monitor the usage of charging stations and determine if more stations are needed or if existing ones need optimization.
 As a user, I want to recharge a charging point when it runs out of charge so that I can ensure all charging points are full and available for other users to use.
### Actors
Actor 1 - Electric Vehicle Driver:
A person who owns or drives an electric vehicle and requires access to a nearby fully charged station to recharge their vehicle efficiently. They use the app to find available charging points that are ready for use.

Actor 2 - Bristol City Council Representative:
An official from the city council responsible for monitoring the usage of charging stations. They utilize the app to collect data on the status of charging points, helping to analyze trends and determine where additional infrastructure is needed or where existing stations might require maintenance.

Actor 3 - Charging Station Technician:
A worker responsible for maintaining and servicing charging points. They use the app to locate stations that are out of power and need to be recharged, allowing them to swap out empty batteries with fully charged ones and ensure stations are functional for users.

### Use Cases
TODO: Describe each use case (at least one per team member).
    Give each use case a unique ID, e.g. UC1, UC2, ...
    Summarise these using the use-case template below.

|  UC1| USE-CASE NAME | 
| -------------------------------------- | ------------------- |
| **Description** | The goal is for the electric vehicle driver to easily locate an available and fully charged charging station without wasting energy traveling between multiple stations. |
| **Actors** | EV Driver|
| **Assumptions** |Use the app to locate nearest available charging point
| **Steps** | In case of errors, the app could direct users to nearby charging points or notify them of issues like server downtime or technical malfunctions. |
| **Variations** | Different stations might display varying levels of information e.g., some stations may show real-time availability, while others might update less frequently. |
| **Non-functional** |  List of qualities the system must have to ensure it works properly.|
| **Issues** | 	List of problems that still need to be addressed.|


|  UC2| USE-CASE NAME | 
| -------------------------------------- | ------------------- |
| **Description** |The representative analyzes station information to estimate use and identify maintenance needs.|
| **Actors** | Actors Council Representative|
| **Assumptions**  | The representative can view data on all charging stations in the application. |
| **Steps** |Log in, view station status, review data, identify trends, and arrange maintenance or improvement.|
| **Variations** | Data is filtered by location, date/time, or station type to support analysis.|
| **Non-functional** | The application needs to be intuitive, responsive, and handle large sets of data efficiently.|
| **Issues** | Giving accurate, up-to-date information and managing trends across a large number of stations.|


|  UC3| USE-CASE NAME | 
| -------------------------------------- | ------------------- |
| **Description** |The technician uses the app to find, service, and update stations requiring work.|
| **Actors** | Charging Station Technician|
| **Assumptions**  |Technicians have access to all station information for servicing and repair.|
| **Steps** |Log in, find stations needing service, visit, replace batteries, fix issues, and update app.|
| **Variations** |tCertain stations may require more extensive servicing than battery replacement.|
| **Non-functional** | The app must be user-friendly and update station status quickly.
Issues|
| **Issues** | Real-time updates and maintenance history tracking delays can create confusion.|

TODO: Your Use-Case diagram should include all use-cases.

![image](https://github.com/user-attachments/assets/9744436f-6b5e-4a76-ba7f-ad7186038084)


## Software Requirements Specification
### Functional requirements
 
FR1: The System should show a clear marking for all the ev ports on the map

FR2: The system should require access to the users location

FR3: They system should show the availibilty on the ports that the user is looking at

FR4: The system should show the price of how much it cost to charge the vehicle

### Non-Functional Requirements

NFR1: The app should quickly respond to the user when used (performance efficiency) 

NFR2: The app should clearly show all the points with suitable sized marking (usability)

NFR3: The app should be usable on chrome internet browsers (compatibillity)

NFR4: The app should have a suitable default location if there is no location provided by the user (reliability)

NFR5: The app should be update to make sure there are working ev ports on all the marked locations on the app (functional suitability)

NFR6: The app should respond to the users request in quick timing (performance efficiency)

NFR7: The app should be able to be used on mobile as well as other devices (portability)

NFR8:The app should should keep users safe just incase they get into a accident this can reported easily.eg time and place (security)

NFR9:The app should maintain frequent updates for users to see once they open the app like available pumps (maintainability) 

Kalid Ahmed
