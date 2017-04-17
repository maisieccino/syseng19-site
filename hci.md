---
layout: page
title: "Human Computer Interaction"
permalink: /hci/
navigation: true
order: 3
---

This page highlights the design of the user interface and user experience of the front end system. This includes initial sketches, wireframes and also first prototype of our application. There are also screen shots of the some of the key pages of the <strong>final product</strong>.

<a href="#initial-sketch" style="margin-top: 7px;" class="btn btn-primary">Initial sketches</a>
<a href="#wireframes" style="margin-top: 7px;" class="btn btn-primary">Initial Mockup</a>
<a href="#hci-principles" style="margin-top: 7px;" class="btn btn-primary">HCI Principles</a>
<a href="#final-screenshot-section" style="margin-top: 7px;" class="btn btn-primary">Screenshots of Final Product</a>

<h3 class="section-header" id="initial-sketch">Initial sketches</h3>
During the beginning stages of developing the user interface, we sketched out some ideas on how the various screens/pages/views will look layout-wise. We decided that the system will have 6 main pages, 1 for user authentication, a clean and user friendly home page, and also 4 other pages for the application process.

<p><img src="{{ site.baseurl }}/assets/img/first-sketch.JPG" class="image" alt="first sketch" height="55%" width="60%"></p>

<h3 class="section-header" id="wireframes">Initial Mockups</h3>
After sketching out how we think the layout of the different views should be, we proceeded to produce the first wireframe; creating cleaner and clearer overviews of the layouts. The wireframes/mockups were designed using Ionic Creator.

There are 5 main layouts for the mockup. The first is the user authentication pages where users create an account to use the application. The second page is the landing page which is where users can choose to enrol in any of the available mentorship programs. When the user selects a mentorship program, there would be a page that shows the details and information of that specific program. After that the user will have to enter their respective interests so that the system can match them to a mentor or mentee. Users can also manually enter some of their interests if it is not available in the selection. Finally the process of application is the confirmation page, where users choose to register themselves as a mentor or mentee. **(Please click to enlarge images)**

<div class="row">
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/signup.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Authentication page</p>
	</div>
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/home.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Landing page</p>
	</div>
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/overview.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Overview of mentorship program</p>
	</div>
</div>
<div class="row">
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/interest.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Application page(Entering interests)</p>
	</div>
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/confirmation.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Confirmation page</p>
	</div>
</div>

<a href="#top" class="btn btn-primary">^ Back to top</a>

<h3 class="section-header" id="first-prototype">First Prototype</h3>
We decided to create the first prototype of the user interface. This prototype builds on what we have got from the wireframes, adding links between the different views and responsive elements such as drop-down menus and tick-boxes to demonstrate how those elements work. However, this prototype does not aim to represent the visual design of the UI. A link to the interactive Ionic prototype is available below.

<a href="https://creator.ionic.io/share/23059853fc12" target="blank" style="margin-top: 7px;" class="btn btn-info btn-lg">First prototype</a>

<h3 class="section-header" id="hci-principles">HCI Principles</h3>
While designing the UI, we focused on anticipating the needs of our user and ensuring that the interface has elements that are easy to access, understand and use to facilitate those actions. While choosing elements to use within our interface, we tried to be as consistent and as possible to acheive a UI that supports efficiency, task completion and user satisfaction. The ways that we were able to acheive this were:

<span class="lead sub-header">Visibility</span><br>
In order to achieve visibility, we made sure that elements were laid out in a manner that makes it obvious for what they are used for. We tried to keep elements in large sections and position important information at a centre location. We also try to arrange elements in an orderly row and column system. Icons were also used to help express specific functionalities. An example of this would be our home page where we listed individual programs clearly and indicating <strong>clearly</strong> which programs they were registered in and which programs that were available.

<div class="row">
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/home-page-final.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Home Page display</p>
	</div>
</div>

<span class="lead sub-header">Feedback</span><br>
This is when the users presses a button and the system reacts in a manner that clearly communicates what has just been accomplished. In order to achieve this, we used functionalities such as hovers on buttons and links and pop ups. We also try to incorporate toast notifications whenever an important action is completed for example after the creation of cohorts/programmes and after registering for a programme. We also implemented ‘alerts’ when users are performing something critical to ensure users don’t do anything undesired unintentionally. An example of this would be an alert box to make sure that admins want to <strong>delete</strong> mentor programmes or cohorts.

<div class="row">
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/restriction-delete-program.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Alert before delete programme</p>
	</div>
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/restriction-delete-cohort.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Alert before delete cohort</p>
	</div>
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/login-restriction.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Fail login Feedback</p>
	</div>
</div>

<span class="lead sub-header">Consistency</span><br>
We achieved consistency in our UI by making sure that all our structures and elements were consistent. We tried to make sure that every page followed the same general theme. For example, colour themes and font styles and sizes would be maintained throughout the individual pages. Here are some examples of the common design patterns that we used for our forms. 

<div class="row">
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/manage-cohort-final.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Layout of cohort page</p>
	</div>
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/register-program-page1-final.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Layout of registration page 1</p>
	</div>
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/register-program-page2-final.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Layout of registration page 2</p>
	</div>
</div>

<span class="lead sub-header">Constraints</span><br>
We have also designed some constraints when designing our user interface to ensure that users do not perform any undesired actions. For example, users are not supposed to sign up for programmes which have <strong>no active cohorts</strong>. Also, when filling up forms, we ensure that users <strong>fill in all the required details</strong> before they can even submit the form. This is done by disabling buttons and only enabling them once the users have performed the required actions. Below are some examples of constraints that are present in our application to prevent users from doing unwanted actions.

<div class="row">
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/cohort-active-restriction.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Only can register if have <strong>active cohort</strong></p>
	</div>
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/registration-all-fields-restriction.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>All fields required.</p>
	</div>
</div>

<h3 class="section-header" id="final-screenshot-section">Final Screenshots</h3>
Below are some screenshots of how our final product looks like. These are some of the key features that our application has such as a <strong>home page</strong> that allows users to browse through available programs and find out more/register for them. A simple <strong>profile page</strong> that displays basic information about the user. A <strong>notification page</strong> that indicates when a new programme is created, when a cohort is active, when mathcing begins etc. 

<div class="row">
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/home-page-final.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Our Final Home Page (Admins)</p>
	</div>
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/home-nonadmin-final.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Our Final Home Page (Normal User)</p>
	</div>
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/program-details-final.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Program Description page.</p>
	</div>
</div>
<div class="row">
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/profile-final.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Profile page.</p>
	</div>
	<div class="col-md-4">
		<a href="#" class="image-pop-up"><img src="{{ site.baseurl }}/assets/img/notification-final.png" class="image" alt="first sketch" height="30%" width="50%"></a>
		<p>Notifications page.</p>
	</div>
</div>

<a href="#top" class="btn btn-primary">^ Back to top</a>

<!-- Modal for images -->
<div class="modal fade" id="imagemodal" tabindex="-1" role="dialog" aria-labelledby="myModalLabel" aria-hidden="true">
    <div class="modal-dialog">
    	<div class="modal-content">              
      		<div class="modal-body">
      			<button type="button" class="close" data-dismiss="modal"><span aria-hidden="true">&times;</span><span class="sr-only">Close</span></button>
        		<img src="" class="imagepreview" style="width: 90%; height: 60%;" >
      			</div>
    	</div>
    </div>
</div>

<!-- Pop up for images -->
<script>
	$(function() {
		$('.image-pop-up').on('click', function() {
			$('.imagepreview').attr('src', $(this).find('img').attr('src'));
			$('#imagemodal').modal('show');   
		});		
	});
</script>