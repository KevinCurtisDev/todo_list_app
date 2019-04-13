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


## Features
The above user stories were achieved by implementing a form that included radio buttons -allowing the user to choose between life quotes or miscelaneous quotes. There is also an input field allowing the user to choose up to five quotes. The user can click the "generate quote(S)" button or, if they want to quit, the quit button.


## Technologies used
* HTML5
* CSS3
* Vanilla JavaScript

## Design pattern

The design pattern used to build this web application is the Model-View-Controller (MVC) pattern.

## Structure (MVC)


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
![overview](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/ToDoOverview.jgp)

#### Performance
![perormance](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/ToDoperformance.jgp)

#### Best Practices
![best practices](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/ToDoBestPractices.jgp)


#### Accessibility
![accessibility](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/ToDoAccessibility.jgp)

#### SEO
![SEO](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/ToDoSEO.jgp)

#### Progressive Web Application
![PWA](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/ToDoPWA.jgp)

### Competitor ToDo web app analysis results

#### Overview
![overview](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competitorOverview.jgp)

#### Performance
![performance](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competitorPerformance.jgp)

#### Best Practices
![best practices](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competitorBestPractices.jgp)

#### Accessibility
![accessibility](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competitorAccessibility.jgp)

#### SEO
![SEO](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competitorSEO.jgp)

#### Progressive Web Application
![pwa](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competitorPWA.jgp)

## Further enhancements
I would like to connect the quote generator engine to a quotation API endpoint in order to expand the number of possible quotes generated. I would also like to add a few more categories to choose from.