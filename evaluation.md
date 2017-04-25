---
layout: page
title: "Evaluation"
permalink: /evaluation/
navigation: true
order: 6
---

This page consists of a summary of our achievements based on our MoSCoW requirements and a short evaluation of the project as a whole.

<a href="#summary-section" style="margin-top: 7px;" class="btn btn-primary">Summary of Achievements</a>
<a href="#critical-evaluation-section" style="margin-top: 7px;" class="btn btn-primary">Critical Evaluation</a>
<a href="#future-work-section" style="margin-top: 7px;" class="btn btn-primary">Future Work</a>

<h3  class="section-header"  id="summary-section">Summary of achievements</h3>
<span class="lead sub-header">Requirements achieved</span><br>
This is a table of requested functional requirements, priority and the status of completion of each requirement.

<img src="{{ site.baseurl }}/assets/img/requirements-evaluation.png" class="image" alt="Summary of achievements" height="80%" width="80%%"><br>

<span class="lead sub-header">Work Package</span><br>
This is the table which illustrates our work package of term 2.
<img src="{{ site.baseurl }}/assets/img/work-package.png" class="image" alt="Summary of achievements" height="70%" width="70%"><br>

<a href="#top" class="btn btn-primary">^ Back to top</a>

<h3  class="section-header"  id="critical-evaluation-section">Critical Evaluation</h3>
<span class="lead sub-header">Architecture design</span><br>
Overall the team was satisfied with the architecture design of our application. We try to use frameworks which were able to communicate with each other and yet independent with each other so that every team member could work on their individual roles. For the client-side, since Ionic framework with Cordova was used, the web application is suited for mobile phones on Android, IOS and Windows platform. Also Ionic is developed with AngularJS which is a widely used Javascript Framework in the developer community. 

For the server-side, the REST API was written in python using the Django REST Framework with PostgreSQL database to store user data. We thought that this worked well with the client side since endpoints of the REST API were easily incorporated with AngularJS and Django also had very well written documentation which made development easier.

<span class="lead sub-header">User Interface design and user experience</span><br>
We thought that developing the user interface for the web application was quite simple and efficient as the Ionic framework provided us with a variety of UI components to enhance user interaction and provide a clean yet elegant look and feel to the web application. We also thought that using the user interface satisfied a few HCI principles so that users have the best experience when using our application.

<span class="lead sub-header">Functionality</span><br>
As for the functionality of our web application, we were quite satisfied with what we were able to implement so far. We were able to implement features that satisfied all of our key requirements and also some additional requirements. Our client also expressed her satisfaction with the functionalities during our user acceptance tests. However, there were certain functionalities that could have been improved given more time such as maybe including a chat system for mentors and mentees to communicate with each other.

<span class="lead sub-header">Compatibility</span><br>
This was one of the main concerns we had initially when choosing which platform develop the application on. Ultimately, we decided to develop our application on mobile platforms. The Ionic framework allows to develop apps that run on all mobile platforms which we have tested. (Team members were using Android and client was using IOS). Hence, we thought that our application is quite compatible for mobile devices and could be easily be translated into a web browser app as well since it was written in AngularJS.

<span class="lead sub-header">Evaluation of Testing</span><br>
We thought that testing played an important role in ensuring that functionalities we have implemented were working as desired and was bug free. We thought that the technologies used for testing definitely aided us in ensuring development went as smoothly and efficiently as possible. We incorporated as much automated testing as possible to detect any failures or edge cases before pushing new features into production. Ionic View also helped us alot in testing the UI and also allowed us to be able to demo our application to our client.

<span class="lead sub-header">Project Management</span><br>
Overall we were satisfied with how each of the team members worked together and manage the development of this project. We were constantly communicating with each other using Facebook Messenger and used the <strong>Kanban methodology</strong> for our development. We were constantly putting up tasks which were to be done in a given deadline and assigning team members on different tasks so that tasks can be completed as soon as possible. We also used GitHub extensively for version control so that team members were able to collaborate during development. 

<h3  class="section-header" id="future-work-section">Future Work</h3>
Given the limited time that we have had, we were only capable to implement features that satisfied key requirements and some additional features. We thought that if we were given more time, for example 6 months we could have definitely implemented more new features. Features such as a chat system could be implemented so that mentors and mentees could chat with each other internally using our application. Also, tighter restrictions on mentor programmes could be added as well for example having enough experience before a user can join a certain mentor programme.

Besides that, we could also implement a system which could allow mentors and mentees to arrange meetings or meetups internally using our application. This would save mentors alot of time. However, we were overall quite happy with the implemented features given the time we were given as the base of our application has been set up from scratch.

<a href="#top" class="btn btn-primary">^ Back to top</a>
