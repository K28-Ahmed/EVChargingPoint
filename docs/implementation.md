# Implementation

## Introduction

Electric vehicle charging information is utilized by means of the Bristol Open Data implementation. It provides informative data that makes it easy to locate charging points. It includes accurate details like the precise location, charger manufacturer, and whether the charger is located in a public car park. The dataset is in general reliable and accurate but may still have errors or outdated data. The issue can be eradicated by the daily checks and modifications to ensure correctness in the data.
For ease of retrieval of information, we incorporated an API by Bristol Open Data to ensure smooth access to the third-party services. The UI has been developed in a way to ensure smooth ease and experience of the user in the case of charging points searching.


## Project Structure
This is a structure of our project's folder organization, and there are numerous reasons why this is necessary. For instance, one of the primary benefits of using an organized file structure is that it provides a higher level of understanding and efficient organization. With a well-defined folder structure, team members can easily comprehend the project, so that everyone knows where to find specific files or resources, ensuring clarity throughout the project.
```
└── 📁EV Charging Points
    └── index.html
    └── Maps.html
    └── Script.html
    └── Search.html
    └── style.css
```
The project directory contains the necessary EV charging platform files: style.css for web design management, index.html for the home page, Maps.html for station location display, Script.html for interactive functionality, and Search.html for station search.
## Software Architecture
 For this project is a structured to be modular, featuring distinct components for both the frontend and backend. For the frontend, we utilize HTML to organize the content, CSS to enhance its visual appeal, and JavaScript to introduce interactivity. This combination significantly influences the user experience and dictates the overall appearance and functionality of the application.

On the backend, we obtain real-time data regarding EV charging stations from the Bristol Open Data API, ensuring that the information we present is both precise and current.

The project is based on a client-server architecture, where the user interface (client) interacts with the server (the API) to access and display pertinent data. Thanks to the modular design, updating either the frontend or backend to incorporate new features or data is a straightforward process. CHECKKKKKKKKKKKKKKKKKKKKKKKKKKKKKKKK
![Insert your component Diagram here](images/component.png)

## Bristol Open Data API
TODO: Document each query to Bristol Open Data

![UML Class diagrams representing JSON query results](images/class1.png)
TODO: Repeat as necessary

# User guide
TODO: Explain how each use-case works by providing step-by-step screenshots for each use-case. This should be based on a tested scenario.
