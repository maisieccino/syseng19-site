---
layout: post
title:  "System Design"
date:   2016-12-10 00:30:51 +0100
categories: development
---

This page highlights the overall system design of our web application. This is includes a system architecture diagram, a class diagram representing the properties of individual classes and thier relationship with each other and finally a entity relation diagram for out database.  

__MORE__ 

<a href="#system-architecture" style="margin-top: 7px;" class="btn btn-primary">System Architecture Diagram</a>
<a href="#entity-design" style="margin-top: 7px;" class="btn btn-primary">Entity Relationship Diagram</a>
<a href="#class-diagram" style="margin-top: 7px;" class="btn btn-primary">Class Diagram</a>

<h3 class="section-header" id="system-architecture">System Architecture Design</h3>
<img src="{{ site.baseurl }}/assets/img/architecture-design.png" class="image" alt="node.js" height="55%" width="65%"><br>

The above diagram is an conceptual illustration that defines the structure of the overall system of the web application. When designing the system architecture, we focused on identifying the key components that will be used for the client side and server side and also the communication between the client side and server side.

For the client side, we have decided to produce an ionic web application which is stored on the client's device. The application will be developed using <code>AngularJS</code> and also Cordova plugins with the Ionic Framework. For authentication, we have decided to use the Oauth2.0 Implicint Grant flow to generate tokens which will be used to authorize users. The client side will be communicating and obtaining data from the server side using HTTP Requests.

For the server side, we have decided to use the <code>Django REST Framework</code> which allows us to develop a REST API. Django also allows us to develop object models which are used to fetch data from the database. The database we are using is <code>PostgreSQL</code>.

<a href="#top" class="btn btn-primary">^ Back to top</a>

<h3 class="section-header" id="entity-design">Entity Relationship Diagram</h3>
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

<a href="#top" class="btn btn-primary">^ Back to top</a>

<h3 class="section-header" id="class-diagram">Class Diagram</h3>
<img src="{{ site.baseurl }}/assets/img/class-diagram.png" class="image" alt="node.js" height="55%" width="65%"><br>

Above is a class diagram which is a static structured diagram that describes the overall structure of the models in the database. It shows the individual classes of the models along with their attributes, methods and also the relationship with other classes. This model will then be translated into actual code which will be written in python using the Django Framework. 

<a href="#top" class="btn btn-primary">^ Back to top</a>
