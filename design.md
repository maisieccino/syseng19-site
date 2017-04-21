---
layout: page
title: Design
permalink: /design/
navigation: true
order: 4
---
This page highlights the overall system design of our web application. This is includes a system architecture diagram, a class diagram representing the properties of individual classes and thier relationship with each other and finally a entity relation diagram for out database. There is also details about how we implemented our matching algorithm.

<a href="#system-architecture" style="margin-top: 7px;" class="btn btn-primary">System Architecture</a>
<a href="#class-diagram" style="margin-top: 7px;" class="btn btn-primary">Class Diagram</a>
<a href="#entity-design" style="margin-top: 7px;" class="btn btn-primary">Database Design</a>
<a href="#design-pattern-section" style="margin-top: 7px;" class="btn btn-primary">Design Patterns</a>
<a href="#key-implementation-details" style="margin-top: 7px;" class="btn btn-primary">Key Implementation Details</a>
<a href="#development-tools-section" style="margin-top: 7px;" class="btn btn-primary">Development Tools</a>

<h3 class="section-header" id="system-architecture">System Architecture Design</h3>
<img src="{{ site.baseurl }}/assets/img/architecture-design.png" class="image" alt="node.js" height="55%" width="65%"><br>

The above diagram is an conceptual illustration that defines the structure of the overall system of the web application. When designing the system architecture, we focused on identifying the key components that will be used for the client side and server side and also the communication between the client side and server side.

For the client side, we have decided to produce an ionic web application which is stored on the client's device. The application will be developed using <code>AngularJS</code> and also Cordova plugins with the Ionic Framework. For authentication, we have decided to use the Oauth2.0 Implicint Grant flow to generate tokens which will be used to authorize users. The client side will be communicating and obtaining data from the server side using HTTP Requests.

For the server side, we have decided to use the <code>Django REST Framework</code> which allows us to develop a REST API. Django also allows us to develop object models which are used to fetch data from the database. The database we are using is <code>PostgreSQL</code>.

<a href="#top" class="btn btn-primary">^ Back to top</a>

<h3 class="section-header" id="class-diagram">Class Diagram</h3>
<img src="{{ site.baseurl }}/assets/img/class-diagram.png" class="image" alt="node.js" height="55%" width="65%"><br>

Above is a class diagram which is a static structured diagram that describes the overall structure of the models in the database. It shows the individual classes of the models along with their attributes, methods and also the relationship with other classes. This model will then be translated into actual code which will be written in python using the Django Framework. 

<a href="#top" class="btn btn-primary">^ Back to top</a>

<h3 class="section-header" id="entity-design">Database Design (Entity Relationship Diagram)</h3>
<img src="{{ site.baseurl }}/assets/img/entity-relation.png" class="image" alt="node.js" height="55%" width="65%"><br>

The above entity relationship diagram illustrates the relationships of entity sets which are stored in the database. This diagram acts as a guide to aid us in developing the PostgreSQL database. Below is a table providing short descriptions of individual entity sets.

<div class="table-responsive">
	<table class="table table-bordered">
		<thead>
	      	<tr>
	        	<th>Entity</th>
	        	<th>Description</th>
	      	</tr>
    	</thead>
    	<tbody>
		    <tr>
		        <td><strong>User</strong></td>
		        <td>Users are registered using an email address and also has an individual profile which contains details such as First and Last Names, position in ATOS, a short biography, join Date etc</td>
		    </tr>
		    <tr>
		        <td><strong>MentorShip</strong></td>
		        <td>This is a list of users which are registered in a mentor program and are mentors and mentees of ther users.</td>
		    </tr>
		    <tr>
		        <td><strong>Cohort</strong></td>
		        <td>This is the size of the mentor program which acts as a restriction to prevent too many users from registering in a single program.</td>
		    </tr>
		    <tr>
		        <td><strong>Programme</strong></td>
		        <td>This illustrates the mentor program itself. Details such as program description, program banner and also the admin responsible for creating the program is stored.</td>
		    </tr>
		    <tr>
		        <td><strong>Tags</strong></td>
		        <td>This is a list of "tags" which are used to match mentors and mentees.</td>
		    </tr>
		    <tr>
		        <td><strong>Updates and Messages</strong></td>
		        <td>These acts as updates for the user regarding the status in the mentor program they are registered in or are choosing to register in.</td>
		    </tr>
		</tbody>
	</table>
</div> 

<h3 class="section-header" id="design-pattern-section">Design Patterns</h3>
The structure of our web application was primarily designed in a Model-View-Controller manner. When developing the web application, we used AngularJS to design and develop the views and controllers of the web application and the Django REST Framework to design the models. Below is a diagram that is a simple illustration of the MVC design pattern we used

<img src="{{ site.baseurl }}/assets/img/mvc-design-pattern.JPG" class="image" alt="node.js" height="55%" width="65%"><br>

<span class="lead sub-header">Views</span><br>
<img src="{{ site.baseurl }}/assets/img/view-design-pattern.JPG" class="image" alt="node.js" height="300px" width="400px"><br>

Views are essentially what gets displayed on the client side. It consists of html pages which consists of Ionic UI components, CSS style sheets and variables bound from the controller. AngularJS also allows data binding in views, which is very useful in linking our templates with data in the controller. We also have an index.html which is essentially the back-bone of all the html pages. We have also designed a side menu which is included in most pages (except login and register and some other pages). Finally, every individual template will have its main content.

<span class="lead sub-header">Controller</span><br>
The controller acts as a link to the model which fetches data from the models and binds them to the templates which are written in Javascript. For every template, a controller is designed to store variables which are displayed to the client and define functions which are called in the templates. There is also some logic implemented with the data obtained from the models to improve user interaction in the client side.  

<span class="lead sub-header">Services and Factories</span><br>
We use AngularJS services and factories as one of the key methods to manage the flow of data between controllers. Some Javascript classes are also designed here which are used to represent data obtained from the models (For example user data, programme data, cohorts etc). We have also designed a factory which acts as an injector to concatenate the currently logged in user authentication token whenever a http request is made. This makes code cleaner, readable, consistent and reduces redundancy.  

<span class="lead sub-header">Directives</span><br>
We also designed some custom directives to extend the functionality of our HTML template pages. The functions written in the directives can be called and binded in to the HTML templates. One example of a function was the “Read More” function which allows users to toggle long text and display/hide them. 

<span class="lead sub-header">Model</span><br>
Our model is responsible for managing the data of the application. Our model is written in python using the Django REST Framework and PostgreSQL is used to implement the database tables. The server side logic is also implemented on the model for example our matching algorithm and management of programme and cohorts. The model also responds to request from the controller to updates itself.

<h3 class="section-header" id="key-implementation-details">Implementation details of key functionalities</h3>

<span class="lead sub-header">Matching Algorithm</span><br>
This section highlights the approach that we used to implement the main matching algorithm that matches mentors and mentees automatically based on their interests. For the input, the algorithm will accept two lists, Mentors and Mentees, containing users. Users have a name, as well as a list of tags. The output would be a list of matches between a mentee and their top three mentors with similar interests.

For every cohort created by an admin, there will be an open and closed date specified which is essentially when the programme is ‘open’ for registration. After the closing date, a ‘Match Date’ is specified and matching will begin at this day. Mentees will be invited to choose their top 3 mentors at this point. Below is a walkthrough of the different stages of our matching algorithm.

<span class="lead sub-header">Stage 1</span><br>
<img src="{{ site.baseurl }}/assets/img/match-stage-1.JPG" class="image" alt="node.js" height="35%" width="50%"><br>

The algorithm will iterate through each mentee in turn. It will look at each mentor, and pair them based on how many similar tags both individuals have. A score will be assigned to each mentor based on how many similar tags they have with the mentee. By the end of this process, for each mentee, there should be a list of mentors and their scores. These should be sorted by the highest score first and the top three mentors with the highest score is chosen.

<span class="lead sub-header">Stage 2</span><br>
<img src="{{ site.baseurl }}/assets/img/match-stage-2.JPG" class="image" alt="node.js" height="20%" width="35%"><br>
Each mentee then will be presented with their top three mentors. They will be invited to sort these according to preference and once these have all been completed, the next stage will begin. Mentees will have 1 day to choose their top 3 mentors which is the “Matching Date” specified when a cohort is created by an admin.

<span class="lead sub-header">Stage 3</span><br>
The algorithm will now implement a version of the Gale-Shapley Algorithm to find an optimal set of matches given the mentee’s preferences. Pairs with highest scores are matched and algorithm will iterate until all mentees have found a suitable match with a mentor. Once this algorithm is run, the matches are then sent to the database to be saved.

<a href="#top" class="btn btn-primary">^ Back to top</a>

<h3 class="section-header" id="development-tools-section">Development Tools</h3>
This section includes all of the tools we have used to manage our project. This includes communication, file storage, UI Design, version control and others and others.

<img src="{{ site.baseurl }}/assets/img/facebook.png" class="image" alt="facebook messenger" height="120" width="120"><br>

<span class="lead sub-header">Facebook Messenger</span><br>
During our first meeting we decided to set up a facebook messenger group as the main tool for communication between each other. We used Facebook Messenger as the main platform to share our ideas and help each other with any problems. 

<img src="{{ site.baseurl }}/assets/img/trello.png" class="image" alt="trello" height="65" width="180"><br>

<span class="lead sub-header">Trello</span><br>
Trello is a collabration tool that organizes our projects on several boards. In our team we divided boards into three parts: Backlog, In progress and Completed. We create tasks by making boards and then add it into the Backlog section, for every task we assign a due date, members responsible for that task and add labels on it to indicate urgency. Once we start working on a task the card would be moved into the in progress section. The team agreed to take a maximum of 6 tasks in progress every week.

<img src="{{ site.baseurl }}/assets/img/github.png" class="image" alt="github" height="65" width="180"><br>

<span class="lead sub-header">Github</span><br>
Github is a version-control service based on git. Our team built three github repositories: one for documentation, main code repository, one repository for the project website. Through github each team member could work separately on same project simultaneously by making branches of master branch and send pull requst to merge each one’s work. Also the version control through github could help us to review our work thus find problems in previous work. 

<img src="{{ site.baseurl }}/assets/img/google-drive.png" class="image" alt="google drive" height="70" width="170"><br>

<span class="lead sub-header">Google drive and Google docs</span><br>
All of the documentation we have completed so far (which includes bi-weekly reports, research, design) are shared in google drive before converting it into Latex for submission or adding the content to the project website.

<img src="{{ site.baseurl }}/assets/img/ionic-creator.png" class="image" alt="google drive" height="70" width="170"><br>

<span class="lead sub-header">Ionic Creator (UI Design)</span><br>
We used Ionic Creator to create the first prototype of our web application. This prototype was presented to our client at the start of term 2. Upon the approval of our client, we have used this prototype as the basis of our UI design. We did make some minor change based on feedback from our client. The purpose of Ionic Creator was to create light-weight simple prototypes that acts as a guide for UI development for the final product. 

<a href="#top" class="btn btn-primary">^ Back to top</a> 