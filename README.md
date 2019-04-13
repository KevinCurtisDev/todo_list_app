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

The lighthouse audit performed on the competitor web app revealed relatively low scores accross all checks.

#### Performance
![performance](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competitorPerformance.png)

The performance score showed a particularly long time to interactive. This result is a bit concerning, as the entire premise of the application is based on user interaction. The web app loads advertisements in iframes. This isn't a best practice. It creates extra calls to the server which slow page loading times. This could be mitigated by lazy loading the iframes or choosing an alternative method to display adds.

#### Best Practices
![best practices](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competitorBestPractices.png)

* The web app doesn't use https as it's transfer protocol. This means the web app is vulnerable to man in the middle attacks, whereby  hacker can easily intercept data moving between the user's browser and the web app's server.

* document.write is used. This is something that is only recommended for test purposes during development and should not be done in a production environment. 

* Javascript libraries with known vulnerabilities are used.

Overall, the web app isn't particularly secure and needs to implement best security practices.

#### Accessibility
![accessibility](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competitorAccessibility.png)

Accessibility issues on this web app include contrast ratio issues. This causes problems for people with impaired vision and should be addressed in the initial design of the web app. There are conflicting duplicate IDs used on the page which can cause a number of functionality issues. The iframes used aren't correctly marked. 


#### SEO
![SEO](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competitorSEO.png)

There's a missing viewport meta tag which dramatically decreases SEO. 

#### Progressive Web Application
![pwa](https://github.com/The-masta-blasta/todo_list_app/blob/master/todo-images/competitorPWA.png)

The following points should be addressed in order for the web app to pass a PWA audit:

* Implement HTTPS
* Use a service wroker script
* include a manifest.JSON file
* Include a theme color met tag
* resize content to fit the window size (currently misconfigured)
* Include a viewport meta tag

## Comparison
The competitor web app is slow to load, however it is feature rich and allows for data persistence across multiple devices. It also offers a mobile version of the application that can be downloaded to a mobile device's homescreen and launched from there. Security is a major concern for this web application and should be addressed imediately. 

"Our" ToDo web application is fast to load and simple to use, however, it doesn't persist data beyond the current browser session. This issue could be addressed by hooking the app up to a database on the backend. Alternatively, we could persist data using a service worker script. The best way forward would be to hook the web app up to a database and include a service worker. this way the data could be persisted between sessions and the aapplication could be used offline. once the user reconnects to the internet, indexDB could be used to update the database in the background. 

## Further enhancements
Further enhancements could be made to the ToDo web application by folling the lighthouse audit recommendations. It could also be connected to a database in order to attain datapersistence. A database used in conjunction with a service worker and indexDB would greatly enhance the usability of the application and allow for offline usage.