---
layout: post
title:  "User Interface Development and Design"
date:   2016-12-5 00:30:51 +0100
categories: development
---

This page highlights the design and development of the user interface and user experience of the front end system. This includes initial sketches, wireframes and also first prototype of our application.

__MORE__

<a href="#initial-sketch" style="margin-top: 7px;" class="btn btn-primary">Initial sketches</a>
<a href="#wireframes" style="margin-top: 7px;" class="btn btn-primary">Initial Wireframes</a>
<a href="#hci-principles" style="margin-top: 7px;" class="btn btn-primary">HCI Principles</a>
<a href="#first-prototype" style="margin-top: 7px;" class="btn btn-primary">First prototype</a>

<h3 class="section-header" id="initial-sketch">Initial sketches</h3>
During the beginning stages of developing the user interface, we sketched out some ideas on how the various screens/pages/views will look layout-wise. We decided that the system will have 6 main pages, 1 for user authentication, a clean and user friendly home page, and also 4 other pages for the application process.

<p><img src="{{ site.baseurl }}/assets/img/first-sketch.jpg" class="image" alt="first sketch" height="55%" width="60%"></p>

<a href="#top" class="btn btn-primary">^ Back to top</a>

<h3 class="section-header" id="wireframes">Initial Wireframes</h3>
After sketching out how we think the layout of the different views should be, we proceeded to produce the first wireframe; creating cleaner and clearer overviews of the layouts. The wireframes were designed using Ionic.

There are 5 main layouts for the wireframe. The first is the user authentication pages where users create an account to use the application. The second page is the landing page which is where users can choose to enrol in any of the available mentorship programs. When the user selects a mentorship program, there would be a page that shows the details and information of that specific program. After that the user will have to enter their respective interests so that the system can match them to a mentor or mentee. Users can also manually enter some of their interests if it is not available in the selection. Finally the process of application is the confirmation page, where users choose to register themselves as a mentor or mentee. **(Please click to enlarge images)**

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

<h3 class="section-header" id="hci-principles">HCI Principles</h3>
While designing the UI, we focused on anticipating the needs of our user and ensuring that the interface has elements that are easy to access, understand and use to facilitate those actions. While choosing elements to use within our interface, we tried to be as consistent and as possible to acheive a UI that supports efficiency, task completion and user satisfaction. The ways that we were able to acheive this were:

<span class="lead sub-header">Visibility</span><br>
In order to acheive visibility, we made sure that elements were lay out in a manner that makes it obvious what they are used for. We tried to keep elements in large sections and also position important information at a center location. We also try to arrange elements in an orderly row and column system. Icons were also used to help express specific functionalities. 

<span class="lead sub-header">Feedback</span><br>
This is when the users presses a button and the system reacts in a manner that clearly communicates what has just been accomplished. In order to acheive this, we used functionalities such as hovers on buttons and links and pop ups. We also try to incorporate as much transtition when switching from different pages. 

<span class="lead sub-header">Consistency</span><br>
The main way in which we were able to achieve consistency in our UI, was by making sure that all our structures and elements were consistent. We tried to make sure that every page followed the same general theme. For example, colour themes and font styles and sizes would be maintained throughout the individal pages.  

<a href="#top" class="btn btn-primary">^ Back to top</a>

<h3 class="section-header" id="first-prototype">First Prototype</h3>
We decided to create the first prototype of the user interface. This prototype builds on what we have got from the wireframes, adding links between the different views and responsive elements such as drop-down menus and tick-boxes to demonstrate how those elements work. However, this prototype does not aim to represent the visual design of the UI. A link to the interactive Ionic prototype is available below.

<a href="https://creator.ionic.io/share/23059853fc12" target="blank" style="margin-top: 7px;" class="btn btn-info btn-lg">First prototype</a>

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
