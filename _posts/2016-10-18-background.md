---
layout: post
title:  "Project Background and Initial Considerations"
date:   2016-10-18 00:30:51 +0100
categories: background
---
<h3 class="section-header">Our Client</h3>
**Atos** is a leader in digital services. Serving a global client base, Atos provides Consulting & Systems Integration services, Managed Services & BPO, Cloud operations, Big Data & Cyber-security solutions, as well as transactional services through Worldline, the European leader in the payments and transactional services industry.

__MORE__

Atos are also focused on business technology that powers progress and helps organizations to create their firm of the future. The client we are working with is based at the Nottingham Office.


<h3 class="section-header">Problem Definition</h3>
*	 Atos is a large firm consisting of multiple employees of different skillset and age group working in various departments.
*	 Our client wanted a way that would allow employees in their workplace to help improve each other's skillset.
*	 Our cliet proposed an application that would pair up mentors who are experienced employees with newer employees which acts as their mentees.
*	 The client also addressed the stable marriage problem which is the problem of finding stable matching between the sample size of mentors and mentees.

<h3 class="section-header">Stable Marriage Problem</h3>
The stable marriage problem marriage problem is the problem of finding a stable matching between two equally sized sets of elements given an ordering of preferences for each element. This problem can be modeled by using the employees as an example where there are equal number of employees willing to act as mentors and similarly apply to become a mentee. 

Currently the process of matching a mentor and mentee is done manually by human resources in Atos. Our client wanted an application that does this automatically and is also able to handle non-perfect data size such as when the number of mentors and mentees differ. 


<h3 class="section-header">Project brief</h3>
The brief for our project is to create a system that matches mentors and mentees on behalf of Atos. The system will allow employees to sign up to various company programmes as either a mentor or a mentee, and then once applications are closed the system will use the users' profiles (as well as any constraints the program has) to find the most suitable mentor-mentee matchings.

The brief was deliberately left as open-ended as possible, to allow us to focus on completing the problem rather than working with an unfamiliar technology stack.

<h3 class="section-header">User Interface Considerations</h3>
When meeting our client for the first time, she was favourable of the system being accessible from both her smartphone and laptop/desktop PC. So naturally we decided that a web app would be the best fit for this project. Whether this was to use Angular, Ionic, Meteor or some other framework had not been decided at this point.

Other things to consider included the possibility of receiving notifications, either in the form of push notifications from the app itself, SMS messages sent to a mobile phone, or emails.
