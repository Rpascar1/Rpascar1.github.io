---
layout: post
title:      "Final Redux Project review"
date:       2020-02-19 14:11:24 -0500
permalink:  final_redux_project_review
---

![Imgur](https://i.imgur.com/sFcCJDu.png)



For this project the main requirements to meet are as follows:

1. Your app should have one HTML page to render your react-redux application

2. There should be 2 container components
 
3. There should be 5 stateless components

4. There should be 3 routes
 
5. The Application must make use of react-router and proper RESTful routing 
 
6. Use Redux middleware to respond to and modify state change
 
7. Make use of async actions to send data to and receive data from a server
 
8. Rails API should handle the data persistence. You should be using fetch() within your actions to GET and POST data from your API - do not use jQuery methods.
 
9. Client-side application should handle the display of data with minimal data manipulation
 
10.   Application should have some minimal styling





To run my specific application the following additional npm dependencies were needed.

  "dependencies": 

  "redux": "4.0.5",
    "redux-form": "8.3.0",
    "redux-thunk": "2.3.0",
    "semantic-redux-form-fields": "0.3.8",
    "semantic-ui-react": "0.88.2"

  "devDependencies": 
    "sass": "1.25.0"
 
	

Let's look at a very generalized review about how I handled these tasks.
	
1. The app should have one HTML page to render your react-redux application. 

 This is acomplished via a single index.html file with a root id div element  with an  id="root"  where all rendering will take   place. 

2. There should be 2 container components.

  Since a container component houses other components that work together.  In this app I have used at a minimum:           A header with: icons, the date, signin and out buttons. A footer with: The app name and current year. A patient care    
	report list that displays the list of reports and admin functions

3. There should be 5 stateless components. 
 
  Using redux store a single external state is achieved and accessed using function components and {connect} from        'react-redux' instead of class components and their individual class level states.	
 
4. There should be 3 routes.
 
   I took care have having enough routes by simply having all crud actions. Instead of 3 routes the app has atleast 5              through the use of  Index, Show, Edit, Create, Delete.
 
5. The Application must make use of react-router and proper RESTful routing. 
 
   This was accomplished by namespacing the rails api resources approriately resulting in:

 " http://localhost:300/api/v1/reports"
 
6. Use Redux middleware to respond to and modify state change.
 
   State change is handled with redux thunk.
 
7. Make use of async actions to send data to and receive data from a server.

   Asycronous fetch calls are used for CRUD actions.
 
8.  Rails API should handle the data persistence. You should be using fetch() within your actions to GET and POST data 
 from your API - do not use jQuery methods.
 
   Building from the backend to front I quickly implemented a Rails	API.
 
9.  Client-side application should handle the display of data with minimal data manipulation.
 
   The only Client-side data manipulations is the actuals creation or editing of report data.
 
10.  Application should have some minimal styling.

   Taking advantage of both custom CSS and the Semantic-UI interface, addind some styling 
   was easily achieved.
 
![Imgur](https://imgur.com/mGOAG1h.gif)



												 
												 


