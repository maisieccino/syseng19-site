---
layout: page
title: "Requirements"
permalink: /requirements/
navigation: true
order: 1
---
<a href="#client-section" style="margin-top: 7px;" class="btn btn-primary">Client, Problem Definition</a>
<a href="#moscow-requirements-section" style="margin-top: 7px;" class="btn btn-primary">Requirements</a>
<a href="#use-case-section" style="margin-top: 7px;" class="btn btn-primary">Use Cases</a>

<!-- Client, problem definition -->
<h3 class="section-header" id="client-section">Our Client</h3>
<p><strong>Atos</strong> is a leader in digital services. Serving a global client base, Atos provides Consulting & Systems Integration services, Managed Services & BPO, Cloud operations, Big Data & Cyber-security solutions, as well as transactional services through Worldline, the European leader in the payments and transactional services industry.</p>
<p>Atos are also focused on business technology that powers progress and helps organizations to create their firm of the future. The client we are working with is based at the Nottingham Office.</p>

<h3 class="section-header">Problem Definition</h3>
*	 Atos is a large firm consisting of multiple employees of different skillset and age group working in various departments.
*	 Our client wanted a way that would allow employees in their workplace to help improve each other's skillset.
*	 Our cliet proposed an application that would pair up mentors who are experienced employees with newer employees which acts as their mentees.
*	 The client also addressed the stable marriage problem which is the problem of finding stable matching between the sample size of mentors and mentees.

<h3 class="section-header">Stable Marriage Problem</h3>
The stable marriage problem marriage problem is the problem of finding a stable matching between two equally sized sets of elements given an ordering of preferences for each element. This problem can be modeled by using the employees as an example where there are equal number of employees willing to act as mentors and similarly apply to become a mentee. 

Currently the process of matching a mentor and mentee is done manually by human resources in Atos. Our client wanted an application that does this automatically and is also able to handle non-perfect data size such as when the number of mentors and mentees differ. 

<!-- Requirements section -->

<h3 class="section-header" id="moscow-requirements-section">Requirements Gathering</h3>
Before constructing our MosCoW requirements, we decided to communicate as much with our client as possible to ensure that we agree on the list of requirements and deliverables the application must provide by the end of term. We initially drafted a list of requirements during our first meeting with our client when she briefed us about the problem definition and what was expected from us.

After making a draft of the requirements, we constantly emailed our client to get feedback and finalised a list of MosCoW requirements during a meeting. 

<h3 class="section-header">MosCoW Requirements</h3>
<p>This is a list of all the requirements as agreed and finalised with our client. These requirements are subject to change over the course of the development phase of this project.</p>
<div class="table-responsive">
	<table class="table table-bordered">
		<thead>
	      	<tr>
	        	<th>Requirement</th>
	        	<th>Description</th>
	        	<th>Category</th>
	      	</tr>
    	</thead>
    	<tbody>
    		<!-- Must Haves -->
    		<tr class="category-header"><td colspan="3">Must Have</td></tr>
		    <tr>
		       	<td>Matching system</td>
		        <td>There must be a matching algorithm that matches mentors and mentees as best as possible according to their preferences.</td>
		        <td>Functional</td>
		    </tr>
		    <tr>
		       	<td>Preferences for matching</td>
		        <td>There must be a system for mentors and mentees to specify their preferences for matching, for instance interests.</td>
		        <td>Functional</td>
		    </tr>
		    <tr>
		        <td>Separate mentorship programmes</td>
		        <td>The system must allow for a number of separate mentorship programmes with their own matching constraints.</td>
		        <td>Non-Functional</td>
		    </tr>
		    <tr>
		        <td>Personal status</td>
		        <td>Users must be able to see the status of their mentorships, for instance whether they can match with users and how active the mentorship is.</td>
		        <td>Functional</td>
		    </tr>
		    <tr>
		        <td>Web Application</td>
		        <td>A complete web application must be provided by the end of the development phase which includes a client side user interface and a functional server back end</td>
		        <td>Functional</td>
		    </tr>
		    <tr>
		        <td>User Interface and Usability</td>
		        <td>The application must operate on a user friendly interface which is simple to use</td>
		        <td>Non-Functional</td>
		    </tr>
		    <!-- Should Have -->
		    <tr class="category-header"><td colspan="3">Should Have</td></tr>
		    <tr>
		       	<td>Profile system</td>
		        <td>Users should be able to create and manage a simple profile so that other users can learn about them. Should include name, image and perhaps a short bio.</td>
		        <td>Functional</td>
		    </tr>
		    <tr>
		       	<td>Notifications</td>
		        <td>Users should be able to receive notifications about key features of the app, for instance when matches are allocated. Should also work across different form factors</td>
		        <td>Functional</td>
		    </tr>
		    <tr>
		        <td>Admin bulk operation interface</td>
		        <td>There should be an interface that allows admins to perform bulk create/read/update/destroy (CRUD) operatons easily.</td>
		        <td>Functional</td>
		    </tr>
		    <!-- Could Have -->
		    <tr class="category-header"><td colspan="3">Could Have</td></tr>
		    <tr>
		        <td>Mentorship meeting record</td>
		        <td>The app could be able to store records of the mentor and mentee meeting each other during the course of the mentorship, with the ability to add comments to this.</td>
		        <td>Functional</td>
		    </tr>
		    <tr>
		        <td>Notifications to meet</td>
		        <td>The app could facilitate instant messaging betweenmentors and mentees.</td>
		        <td>Functional</td>
		    </tr>
		    <!-- Would Have -->
		    <tr class="category-header"><td colspan="3">Would Have</td></tr>
		     <tr>
		        <td>Corporate Directory Lookup</td>
		        <td>The app would be able to use the company’s internal “Corporate Directory” to populate users’ profiles</td>
		        <td>Functional</td>
		    </tr>
		    <tr>
		        <td>Instant messaging</td>
		        <td>The app could be able to store records of the mentor and mentee meeting each other during the course of the mentorship, with the ability to add comments to this.</td>
		        <td>Functional</td>
		    </tr>
		</tbody>
	</table>
</div>

<a href="#top" class="btn btn-primary">^ Back to top</a>

<!-- Use Case Section -->
<h3 class="section-header" id="use-case-section">Use Cases</h3>
This is a list of use cases which aims to illustrate the interaction between users at different parts of the application. 

<div class="table-responsive decisionTable"> 
	<table class="table table-bordered">
		<thead>
	      	<tr>
	        	<th>Use case ID</th>
	        	<th>Use Case Name</th>
	      	</tr>
    	</thead>
    	<tbody>
    		<col width="20%">
  			<col width="80%">    		
		    <tr>
		       	<td>UC1</td>
		        <td>Create Account</td>		        
		    </tr>
		    <tr>
		       	<td>UC2</td>
		        <td>Explore information of program</td>		        
		    </tr>
		    <tr>
		       	<td>UC3</td>
		        <td>Register for a mentorship program</td>		        
		    </tr>
		    <tr>
		       	<td>UC4</td>
		        <td>Manage Mentor Programme</td>		        
		    </tr>
		    <tr>
		       	<td>UC5</td>
		        <td>Manage Cohorts</td>		        
		    </tr>
		    <tr>
		       	<td>UC6</td>
		        <td>Notification System</td>		        
		    </tr>
		    <tr>
		       	<td>UC7</td>
		        <td>Check individual profile</td> 
		    </tr>
		    <tr>
		       	<td>UC8</td>
		        <td>Edit profile</td> 
		    </tr>
		    <tr>
		       	<td>UC9</td>		        
		        <td>List user's mentors or mentees</td>		        	        
		    </tr>
		</tbody>
	</table>
<br>
	<table class="table table-bordered">  <!-- Usecase1 -->
		<thead>
			<tr>
				<th>USE CASE</th>
				<th>Create Account</th>
			</tr>
		</thead>
		<tbody>
			<col width="20%">
  			<col width="80%">
			<tr>
				<td>ID</td>
				<td>UC1</td>
			</tr>
			<tr>
				<td>BREIF DESCRIPTION</td>
				<td>Allow uses to create their own account and set up basic information </td>
			</tr>
			<tr>
				<td>PRIMARY ACTORS</td>
				<td>User</td>
			</tr>
			<tr>
				<td>PRECONDITIONS</td>
				<td>None</td>
			</tr>
			<tr>
				<td>MAIN FLOW</td>
				<td>
					1.Click 'Create an Account' button.<br/>
					2.Fill the required information in sign up page.<br/>
					3.Click 'Sign up' button
				</td>
			</tr>
			<tr>
				<td>POSTCONDITIONS</td>
				<td>User account is set up and is redirected to home page</td>
			</tr>
		</tbody>
	</table>
<br>
	<table class="table table-bordered"> <!-- 2 -->
		<tbody>
			<col width="20%">
  			<col width="80%">
  			<thead>
				<tr>
					<th>USE CASE</th>
					<th>Find out more about specific mentorship program</th>
				</tr>
			</thead>
			<tr>
				<td>ID</td>
				<td>UC2</td>
			</tr>
			<tr>
				<td>BREIF DESCRIPTION</td>
				<td>Users chooses from the listed mentorship programs to find more information about the mentoring program</td>
			</tr>
			<tr>
				<td>PRIMARY ACTORS</td>
				<td>User</td>
			</tr>
			<tr>
				<td>PRECONDITIONS</td>
				<td>User must be registered and is already signed in</td>
			</tr>
			<tr>
				<td>MAIN FLOW</td>
				<td>
				1.Go to home page<br>
				2.Click on 'Find Out More' for the desired mentorship program which are listed.
				</td>
			</tr>
			<tr>
				<td>POSTCONDITIONS</td>
				<td>User is redirected to a decription page of the specific mentorship program before proceeding to next step.</td>
			</tr>
			
		</tbody>
	</table>
<br>
	<table class="table table-bordered"> <!-- 3 -->
		<tbody>
			<col width="20%">
  			<col width="80%">
			<thead>
				<tr>
					<th>USE CASE</th>
					<th>Resgiter for a mentor program</th>
				</tr>
			</thead>
			<tr>
				<td>ID</td>
				<td>UC3</td>
			</tr>
			<tr>
				<td>BREIF DESCRIPTION</td>
				<td>User registers for mentorship program of their interest.</td>
			</tr>
			<tr>
				<td>PRIMARY ACTORS</td>
				<td>User</td>
			</tr>
			<tr>
				<td>PRECONDITIONS</td>
				<td>User must be logged in to their account</td>
			</tr>
			<tr>
				<td>MAIN FLOW</td>
				<td>
					1.Go to home page<br>
					2.Click on desired mentorship program<br>
					3.Click the 'Register Here' button<br>
					4.Choose the option of signing up as a mentor or mentee <br>
					5.Select tags and interest for matching.
				</td>
			</tr>
			<tr>
				<td>POSTCONDITIONS</td>
				<td>
					1.Redirected back to home page upon successful registration.<br>
				</td>
			</tr>
		</tbody>
	</table>
<br>
	<table class="table table-bordered">
	  <!--  4 -->
		<tbody>
			<col width="20%">
  			<col width="80%">
  			<thead>
				<tr>
					<th>USE CASE</th>
					<th>Manage Mentor Programme</th>
				</tr>
			</thead>
			<tr>
				<td>ID</td>
				<td>UC4</td>
			</tr>
			<tr>
				<td>BREIF DESCRIPTION</td>
				<td>Admin can create a mentor programme which users can register for</td>
			</tr>
			<tr>
				<td>PRIMARY ACTORS</td>
				<td>User(Admin)</td>
			</tr>
			<tr>
				<td>PRECONDITIONS</td>
				<td>
					1.Logged in successfully. User MUST be an Admin.
				</td>
			</tr>
			<tr>
				<td>MAIN FLOW</td>
				<td>
					1.Go to side menu<br>
					2.Select Create Mentor Program<br>
					3.Fill in form details and confirm creation.
				</td>
			</tr>
			<tr>
				<td>POSTCONDITIONS</td>
				<td>New program is created, user is redirected to home page and the new program is listed.</td>
			</tr>
			<tr>
				<td>ALTERNATIVE FLOW</td>
				<td>
					1a.Admin decides to edit program.<br>
					1b.Admin decides to delete program. After confirming deletion, program is deleted<br> 
				</td>
			</tr>	
		</tbody>
	</table>
<br>
	<table class="table table-bordered">  <!-- 5 -->
		<tbody>
			<col width="20%">
  			<col width="80%">
  			<thead>
				<tr>
					<th>USE CASE</th>
					<th>Manage Cohorts</th>
				</tr>
			</thead>
			<tr>
				<td>ID</td>
				<td>UC5</td>
			</tr>
			<tr>
				<td>BREIF DESCRIPTION</td>
				<td>Admins can create cohort for mentor rogrammes which users can register for.</td>
			</tr>
			<tr>
				<td>PRIMARY ACTORS</td>
				<td>User(Admin)</td>
			</tr>
			<tr>
				<td>PRECONDITIONS</td>
				<td>Logged in successfully. User MUST be an admin</td>
			</tr>
			<tr>
				<td>MAIN FLOW</td>
				<td>
					1.On home page, click on cohort button of desired mentor programme<br>
					2.Fill in open date, close date and match date<br>
					3.Confirm to create program
				</td>
			</tr>
			<tr>
				<td>POSTCONDITIONS</td>
				<td>New cohort is created. Admins can go to cohort page and a new cohort is listed.</td>
			</tr>
			<tr>
				<td>ALTERNATIVE FLOW</td>
				<td>
					1a.Admin decides to edit a cohort. Admins clicks on edit cohort, and changes cohort details.<br>
					1b.Admin decides to delete cohort. Admin clicks on delete cohort button, after confirming, program is deleted.
				</td>
			</tr>	
		</tbody>
	</table>
<br>
	<table class="table table-bordered">  <!-- 6 -->
		<tbody>
			<col width="20%">
  			<col width="80%">
  			<thead>
				<tr>
					<th>USE CASE</th>
					<th>Notification system for mentor and mentee</th>
				</tr>
			</thead>
			<tr>
				<td>ID</td>
				<td>UC6</td>
			</tr>
			<tr>
				<td>BREIF DESCRIPTION</td>
				<td>Users can receive notifications when new programs are created and if the current date is the matching date.</td>
			</tr>
			<tr>
				<td>PRIMARY ACTORS</td>
				<td>User</td>
			</tr>
			<tr>
				<td>PRECONDITIONS</td>
				<td>User is registered and logged in successfully</td>
			</tr>
			<tr>
				<td>MAIN FLOW</td>
				<td>
					1.Go to home page<br>
					2.On the tab bar go to notifications<br>
				</td>
			</tr>
			<tr>
				<td>POSTCONDITIONS</td>
				<td>Users can see any notifications from their mentee or mentor</td>
			</tr>
		</tbody>
	</table>
<br>
	<table class="table table-bordered">  <!-- 7 -->
		<tbody>
			<col width="20%">
  			<col width="80%">
  			<thead>
				<tr>
					<th>USE CASE</th>
					<th>Check individual profile</th>
				</tr>
			</thead>
			<tr>
				<td>ID</td>
				<td>UC7</td>
			</tr>
			<tr>
				<td>BREIF DESCRIPTION</td>
				<td>Users could see information about themselves which includes current role and current enrolled programs.</td>
			</tr>
			<tr>
				<td>PRIMARY ACTORS</td>
				<td>User</td>
			</tr>
			<tr>
				<td>PRECONDITIONS</td>
				<td>Logged in successfully</td>
			</tr>
			<tr>
				<td>MAIN FLOW</td>
				<td>
					1.Go to home page<br>
					2.On tab bar click 'Profile'<br>
				</td>
			</tr>
			<tr>
				<td>POSTCONDITIONS</td>
				<td>Users could see their own profiles along with its details.</td>
			</tr>
		</tbody>
	</table>
<br>
	<table class="table table-bordered">  <!-- 8 -->
		<tbody>
			<col width="20%">
  			<col width="80%">
  			<thead>
				<tr>
					<th>USE CASE</th>
					<th>Edit user profile</th>
				</tr>
			</thead>
			<tr>
				<td>ID</td>
				<td>UC8</td>
			</tr>
			<tr>
				<td>BREIF DESCRIPTION</td>
				<td>Users can edit their profile if needed</td>
			</tr>
			<tr>
				<td>PRIMARY ACTORS</td>
				<td>User</td>
			</tr>
			<tr>
				<td>PRECONDITIONS</td>
				<td>Logged in successfully </td>
			</tr>
			<tr>
				<td>MAIN FLOW</td>
				<td>
					1.Go to home page<br>
					2.Click the side-bar menu<br>
					3.Click 'Settings' button.
				</td>
			</tr>
			<tr>
				<td>POSTCONDITIONS</td>
				<td>User is redirected to profile page with profile details edited.</td>
			</tr>
		</tbody>
	</table>
	<table class="table table-bordered">  <!-- 8 -->
		<tbody>
			<col width="20%">
  			<col width="80%">
  			<thead>
				<tr>
					<th>USE CASE</th>
					<th>List user's mentors or mentees</th>
				</tr>
			</thead>
			<tr>
				<td>ID</td>
				<td>UC9</td>
			</tr>
			<tr>
				<td>BREIF DESCRIPTION</td>
				<td>Users can see a list of their mentor or mentees in different mentor programs</td>
			</tr>
			<tr>
				<td>PRIMARY ACTORS</td>
				<td>User</td>
			</tr>
			<tr>
				<td>PRECONDITIONS</td>
				<td>Logged in successfully </td>
			</tr>
			<tr>
				<td>MAIN FLOW</td>
				<td>
					1.Go to home page<br>
					2.Click the side-bar menu<br>
					3.Click 'My mentors' button or 'My mentees' button.
				</td>
			</tr>
			<tr>
				<td>POSTCONDITIONS</td>
				<td>A list of the currenty logged in user's mentors and mentees is displayed according to their respective mentor programs.</td>
			</tr>
		</tbody>
	</table>
</div>

<a href="#top" class="btn btn-primary">^ Back to top</a>