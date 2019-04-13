# TODO WEB APP
## Summary

The ToDo web application is a simple browser based ToDo list, built with vanilla JavaScript, html5 and css3. It uses a Model View Controller (MVC) structure and was developed using a Test Driven Devlopment (TDD) approach (with the jasmine framework). The appication allows a user to add a new todo, edit or delete an existing todo, or select all todos at once and then delete them if desired. The user can also view completed or incompleted ToDos.

You can try the ToDo web application live here: [TODO WEB APP](https://the-masta-blasta.github.io/todo_list_app/)


## UX
The ToDo web app was built with simplicity in mind. It is a single page web application, which allows for easy navigation. Because of the minimal use of css and the absence of large files or images, the application loads and responds to user inputs with exceptional speed - further enhancing the user experience.

### User stories: 
The following user stories were used when building the ToDo web application:

As a user of the ToDo we app, I want to... 
* ..add a new ToDo. 
* ..edit an existing ToDo.
* ..delete an existing ToDo.
* ..select one or many existing ToDos.
* ..delete all ToDos in one go.
* ..view completed ToDos.
* ..view active (incomplete) ToDos.


## Technologies used
* HTML5
* CSS3
* Vanilla JavaScript

## Design pattern and file structure (MVC)

The design pattern used to build this web application is the Model-View-Controller (MVC) pattern.


## Testing
Manual testing was carried out, using a python http server, applying the listed user stories above. 

The Jasmin testing framework was used in order to build the application with a test driven development methodology.

### Jasmine Testing details


## Deployment
The app was deployed on github pages and can be viewed at the following link: [TODO WEB APP](https://the-masta-blasta.github.io/todo_list_app/)

In order to view the jasmine tests you can clone or download the github repo to your local machine. You should have python3 installed on your machine. from your terminal or command line CD into the project directory and run a python htp server with the following command: python3 -m http.server 

Once the server is running you can view and use the ToDo app in your browser by visiting the url produced by the python server.

to view the jasmine test suit, add the following extension to the generated url: /SpecRunner.html

## Analysis and comparison of ToDo web app with competitor web app
Google's lighthouse audit was used for my analyis and comparison of the ToDo web app and a competitor ToDo web app. 

The competitor web app can be viewed at the the following url: [http://todolistme.net/](http://todolistme.net/)

### ToDo web app analysis results

#### Overview

The Todo web app is a browser based web application, and is not connected to a backend database.

![overview](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/ToDoOverview.png)

The lighthouse audit overview scores positively in the areas of performance and best practices. There are however quite a few improvements that can be made to the ToDo web app in the areas of Accesibility, SEO, and PWA (progressive web app).

#### Performance
![perormance](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/ToDoperformance.png)

Performance scores are excellent, with no areas in need of improvement. This is due to the ToDo app not needing to load any large scripts or image files.

#### Best Practices
![best practices](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/ToDoBestPractices.png)

There was one error recorded in the console with regard to a javascript file not being found. This particular error is negligable as the file in question is used for the jasmine test environment, which is seperate from the running of the ToDo app. This error may be mitigated by removing the link to the file in the index.html file.

#### Accessibility
![accessibility](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/ToDoAccessibility.png)

Accessibility should be improved for users with limited vision and for screen readers. These issues can be resolved by increasing the colour contrast on the page, and by increasing the font size of the small text at the bottom of the page. Aria roles should also be included in order to allow screen readers to navigate through the site in a logical and user friendly order. Reference should be made to WCAG accessibility standards when developing online applications.

#### SEO
![SEO](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/ToDoSEO.png)

In order to ammend the SEO issues the site should include a meta tag stating the viewport dimensions. Font sizes should also be adjusted to fit with W3C web standards. 

#### Progressive Web Application
![PWA](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/ToDoPWA.png)

In order to enhance the ToDo web application with progressive features, the following adjustments should be made:

* Include a service worker (to store content for offline viewing)
* Include a manifest.JSON file (to store information about launching the web app from a mobile phone home screen icon) 
* Include a meta tag in the index.html file refering to the theme color.
* Include a viewport meta tag in the index.html file.
* Use of indexD

### Competitor ToDo web app analysis results

The competitor is a feature rich to web application that runs in the browser, and is supported by a database that allows for data persistence.

#### Overview
![overview](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competirorOverview.png)



#### Performance
![performance](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competitorPerformance.png)

#### Best Practices
![best practices](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competitorBestPractices.png)

#### Accessibility
![accessibility](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competitorAccessibility.png)

#### SEO
![SEO](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competitorSEO.png)

#### Progressive Web Application
![pwa](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competitorPWA.png)

## Further enhancements
Further enhancements could be made to the ToDo web application by folling the lighthouse audit recommendations. It could also be connected to a database in order to attain datapersistence. A database used in conjunction with a service worker and indexDB would greatly enhance the usability of the application and allow for offline usage.