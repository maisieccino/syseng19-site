---
layout: page
title: "Research"
permalink: /research/
navigation: true
order: 2
---
<a href="#platform-research-section" style="margin-top: 7px;" class="btn btn-primary">Potential Platform Research</a>
<a href="#technical-research-section" style="margin-top: 7px;" class="btn btn-primary">Technical Research</a>
<a href="#algorithm-research-section" style="margin-top: 7px;" class="btn btn-primary">Algorithm Research</a>
<a href="#summary-decision-section" style="margin-top: 7px;" class="btn btn-primary">Summary of our decisions</a>

<!-- Platform Research Section -->
<h3 class="section-header" id="platform-research-section">Potential Platforms Reseach</h3>
<img src="{{ site.baseurl }}/assets/img/mobile-vs-browser.jpg" class="image" alt="node.js" height="120" width="200"><br>

During the first meeting with our client, she made it clear to us initially that she would prefer this application to be used on the web browser or mobile device. Therefore, the team decided to undergo some research and discuss the advantages and the drawbacks of each platform.

<span class="lead sub-header">Web Browser</span><br>
Web browsers would allow us to implement more advanced features which mobile platforms cannot provide due to the existence of many <code>Javascript</code> libraries such as <code>ReactJS EmberJS, Jquery</code> etc. However, in terms of accessibility, mobile application might be more convenient as native mobile apps does not need to be accessed by using the web browser. 

<span class="lead sub-header">Mobile Application</span><br>
Since our client wanted it to be a web application, choices are limited to only <code>AngularJS</code> and <code>Ionic</code> which allowed us to build native hybrid web applications. Regardless of the limit of choices, we thought that AngularJS provided us with the tools to deliver the key requirements requested by our client. Also, mobile apps are very accessible, since mobile phones are carried around us everywhere, the app can be used anywhere and anytime as long as there is Wifi connection.  

<span class="lead sub-header">Our Decision - Hybrid Mobile Application</span><br>
Ultimately, we decided to develop a hybrid web application for mobile platforms as we thought that AngularJS and Ionic provided allowed us to build a good application that satisfies the client’s requirements and also allows the application to be very accessible.

<h3 class="section-header" id="technical-research-section">Technical Stack Research</h3>
This section details all the technical research we have done (excluding architecture) throughout this project, including open-source libraries and frameworks that we considered to use for the final system. Our research was split in to 2 categories which was frontend research and backend research.

<!-- Backend Framework Research sention -->
<span class="lead sub-header"><strong>Backend Framework/Libraries</strong></span><br>

<img src="{{ site.baseurl }}/assets/img/node.jpg" class="image" alt="node.js" height="120" width="120"><br>

<span class="lead sub-header">Node.JS</span><br>
Node.JS is an application framework that runs JavaScript code as a native app on computers. It’s gained extreme popularity over the last couple of years and I myself have used it for a few projects in the past. The community is rather large and there’s a library for pretty much anything.

Node.JS programs are written using JavaScript, a dynamic, untyped language developed originally for scripting web pages in the browser. Recent versions of the language have introduced classes and other useful features, but it’s type inferencing has some weird side effects <code>(try {} == [] and [] == {})</code>.

<span class="lead sub-header">Advantages</span>
*	Large developer community with plenty of libraries.
*	Easy to write and deploy code.
*	Shares a common language with web page scripts.
*	Object variables - JavaScript internally uses hashes/dictionaries/key-value pairs to represent objects, and the value can be of any type… even functions. Makes for very quick development.
*	Event-driven - your Node app can do other things while waiting for asynchronous operations (disk I/O, http requests, etc) which can make up for only having one thread.

<span class="lead sub-header">Disadvantages</span>
*	Single threaded - no concurrency features.
*	Callbacks - a comment paradigm of JavaScript is using callbacks: functions that accept another function which is called once the original function completes. It can often lead to very messy code, with five or six functions nested inside each other.

<!-- Ruby on Rails -->
<img src="{{ site.baseurl }}/assets/img/ruby.jpg" class="image" alt="node.js" height="120" width="100"><br>

<span class="lead sub-header">Ruby On Rails</span><br>
Ruby on Rails is a web framework that’s written in Ruby, a dynamic programming language. It relies heavily on scaffolding, and the directory/fire structure is rather rigid. However, it means that applications are developed very quickly, and is often used as a prototyping framework.

The Ruby language is extremely expressive, allowing functions to be written relatively fast without worrying too much about low level features like memory management. Also, like with Node.JS, Ruby has a large developer following and library, using the Rubygems service.

<span class="lead sub-header">Advantages</span>
*	Fast development time thanks to a readable, dynamic language. Ruby trades off some processing overhead in lieu of developer satisfaction.
*	Rails uses scaffold code to generate projects very quickly, and tasks like page routing, templating and database ORM (object relation model, where a row in a database table is represented with a language’s class) are built in.
*	Ruby contains symbols that can be used instead of strings for hash keys. For instance, <code>:id</code> could represent the id of a user.

<span class="lead sub-header">Disadvantages</span>
*	Scaffolding can mean that the project structure is inflexible, and code should be distributed between files as the Rails developers intended.
*	Ruby’s dynamic nature can mean that it runs a little slower than compiled/statically typed languages, as there’s overhead resulting from Ruby’s type inference engine.

<img src="{{ site.baseurl }}/assets/img/django.jpg" class="image" alt="node.js" height="75" width="200"><br>

<span class="lead sub-header">Django</span><br>
Django is a high level web framework that is written in python  that encourages rapid development. Django is also free and open source and is built by experienced developers which takes care of much hassle of certain parts of web development. One of the main advantages of Django is that it is really fast and is designed to help developers take applications from concept to completion very quickly.  

<span class="lead sub-header">Advantages</span>
*	Very fast - Most of the aspects of web development are taken care of by the framework itself such as user authentication and form handling. It also has an inbuilt User Model implementation.
*	Security - Django’s inbuilt user authentication system are reassuringly secure which helps developers avoid security mistakes.
*	Scalability - Despite many in built system takes makes development really fast, Django is exceedingly scalable and flexible.

<span class="lead sub-header">Disadvantages</span>
*	Maintainability - Since Django runs on python, it needs to maintain backwards compatibility when there are newer versions of python which makes it evolve slowly.
*	Templating - Most inbuilt features in Django require the use of templates, which can be rigid to the developer when trying to implement something different.  

<img src="{{ site.baseurl }}/assets/img/revel.jpg" class="image" alt="node.js" height="60" width="140"><br>

<span class="lead sub-header">Revel</span><br>
Revel is a web framework written using the Go language, a statically and strongly typed language. Go’s main benefits are its strong concurrency and networking features, and is high level enough to hide things like memory management.

The Revel framework is similar to Ruby on Rails in that it employs the MVC (model, view, controller) design pattern to structure the project. It can be used for serving HTML from templates, or it can be also used for serving a RESTful JSON API.

<span class="lead sub-header">Advantages</span>
*	Statically and strongly typed - the Go language may not have the syntactic sugar of Ruby or Python, but it’s built to run fast. 
*	Multithreading - Go uses channels to handle concurrent features, which can be used to create more optimised servers, if needed.

<span class="lead sub-header">Disadvantages</span>
*	Barebones - as Revel is very lightweight, it also means that the developer needs to implement a lot of features themselves, increasing development time.
*	Revel uses scaffolding to generate the project files, which may mean that the project structure is rigid.

<a href="#top" class="btn btn-primary">^ Back to top</a>

<!-- Front end framework section -->
<span class="lead sub-header"><strong>Frontend Framework/Libraries</strong></span><br>

<!-- Angular -->
<img src="{{ site.baseurl }}/assets/img/angularjs.jpg" class="image" alt="node.js" height="120" width="120"><br>

<span class="lead sub-header">AngularJS</span><br>
AngularJS is an open-sourced Javascript framework used for developing single-page web application. It aims to overcome the shortages of HTML for building web application.AngularJS is much closer to model-view-view model pattern. Where model is the data in application, view is what shows to user, view-model provides functions and specific data.

<span class="lead sub-header">Advantages</span>
*	AngularJS is supported by Google and a great development community.
*	AngularJS operate directly on DOM rather than inner HTML, more efficiently.
*	No need to use observable functions.
*	Extended features such as dependency injection, routing, animations, view orchestration, and more.

<span class="lead sub-header">Disadvantages</span>
*	Source code too complex.
*	Not easy to learn how to write your own directive.

<img src="{{ site.baseurl }}/assets/img/ionic.jpg" class="image" alt="node.js" height="70" width="150"><br>

<span class="lead sub-header">Ionic</span><br>
Since one of the requirements of our application was being mobile compatible, we decided to look into Ionic Framework as well. Ionic is a HTML5 SDK (software development kit) used to build hybrid mobile app by using Html, Css and Javascript. By using Ionic Creator, we could build a similar user interface interactions like native mobile app. Ionic is based on AngularJS.

<span class="lead sub-header">Advantages</span>
*	Support cordova plugins to enrich functions in our app.
*	Once produce ionic program it could be run on both IOS and Android development.
*	Powerful CLI tool: Control and manage you project easier.
*	Providing beautiful  UI components.
*	Developing using AngularJS, can use all the modules from angular.

<span class="lead sub-header">Disadvantages</span>
*	Not equal to native app, native device’s API depends on whether Cordova support it.
*	Can not deal with huge amount of images.
*	Some platforms like windows phone are not supported.

<img src="{{ site.baseurl }}/assets/img/bootstrap.jpg" class="image" alt="node.js" height="80" width="160"><br>

<span class="lead sub-header">Bootstrap</span><br>
Bootstrap includes CSS, HTML and JavaScript components. It adheres to responsive web design standards, allowing developers to create responsive sites of all complexities and sizes.

<span class="lead sub-header">Advantages</span>
*	Responsive web design support (can also be disabled if required)
*	Excellent documentation available online
*	Updated continously, hence it includes the latest and best features. It is also upgraded to use Sass as a CSS processor.

<span class="lead sub-header">Disadvantages</span>
*	Out-of-the-box file size of 276kB due to excessive number of rarely used styles
*	Excessive number of HTML classes and DOM elements can be messy and confusing

<img src="{{ site.baseurl }}/assets/img/reactjs.jpg" class="image" alt="node.js" height="70" width="170"><br>

<span class="lead sub-header">React</span><br>
React.js is a JavaScript library for building user interfaces, built by top engineers at Facebook. React is all about reusable components. However, unlike frameworks, which are built with the goal of getting whole apps up and running quickly, the only thing you do with React is build components. As React.js’s core functionality, components make reusing code, testing, and separating concerns easy.

<span class="lead sub-header">Advantages</span>
*	Easy to know how a component is rendered, you just look at the render function.
*	React is able to render on server side.
*	React ensures readability and makes maintainability easier.

<span class="lead sub-header">Disadvantages</span>
*	It's not a full framework. There's no router nor model management libraries built into reactJS -- unlike angular or ember. Hence one needs to have some degree of experience in picking libraries to fulfill these needs.
*	React is rather verbose. Writing components isn't as straight forward as pure HTML & JS

<img src="{{ site.baseurl }}/assets/img/emberjs.jpg" class="image" alt="node.js" height="80" width="160"><br>

<span class="lead sub-header">Ember.Js</span><br>
Ember.js is an open source JavaScript client-side framework for developing the web applications and uses the MVC(Model-View-Controller) architecture pattern. Ember.js is mainly used to creating reusable and maintainable JavaScript web applications.

<span class="lead sub-header">Advantages</span>
*	Ember.js is an open source JavaScript framework under (MIT license).
*	It is a flexible framework that embraces the concept of fast web page. It allows to speed up the performance of your application without reloading the whole page.
*	It has the handlebars templating library which is similar as HTML and also embed an expressions that changes the display.

<span class="lead sub-header">Disadvantages</span>
* 	Very dependant on jQuery libraries. Very few libraries are written from scratch.
*	Less space for customization of everything.
*	No server-side rendering.

<a href="#top" class="btn btn-primary">^ Back to top</a>

<span class="lead sub-header"><strong>Our decision for technology stack</strong></span><br>

<div class="table-responsive">
	<table class="table table-bordered decisionTable">
		<tbody>
			<col width="15%">
  			<col width="85%">
			<tr>
				<td width="100px;"><strong>Decision 1</strong></td>
				<td>Which web application framework do we use for the <strong>front-end?</strong></td>
			</tr>
			<tr>
				<td rowspan="3"><strong>Option Considered</strong></td>
				<td>Angular JS and Ionic</td>
			</tr>	
			<tr><td>React JS</td></tr>
			<tr><td>Ember JS</td></tr>
			<tr>
				<td><strong>Final Decision</strong></td>
				<td>Angular JS and Ionic</td>
			</tr>
			<tr>
				<td><strong>Justifications</strong></td>
				<td>
					<strong>Why not React JS?</strong>
					<p>We considered React JS due to its ability to build components and functionality which are well maintained. React is also able to render on server side which makes integration with backend easier. However, React is not a full framework as there are no router nor model management libraries built into ReactJS. Hence writing components is not as easy.</p>
					<strong>Why not Ember JS</strong>
					<p>We chose Ember JS as it is a flexible framework which speeds up the performance of our application without reloading the whole page. Ember is also good for REST API querying which is what we plan to use for communication with database. However, we have to write our own ajax requests since a lot of ember addons are ports of existing jQuery libraries and very few are written from scartch.</p>
					<strong>Why Angular JS and Ionic</strong>
					<p>The main advantages of Angular is the flexibility and support by the community. Angular JS is supported by Google and has a great development community. It also operates directly on DOM rather than inner HTML more efficiently. Our Client also heavily emphasised that the application should be available on mobile. Ionic is able to produce applications that can run on both IOS and Android environment. It also makes developing with Angular easier because modules from Angular ca be used.</p>
				</td>
			</tr>
		</tbody>
	</table>
</div>

<div class="table-responsive">
	<table class="table table-bordered decisionTable">
		<tbody>
			<col width="15%">
  			<col width="85%">
			<tr>
				<td width="100px;"><strong>Decision 2</strong></td>
				<td>Which web application framework do we use for the <strong>back-end?</strong></td>
			</tr>
			<tr>
				<td rowspan="4"><strong>Option Considered</strong></td>
				<td>Django</td>	
			</tr>
			<tr><td>Ruby On Rails</td></tr>
			<tr><td>Node JS</td></tr>
			<tr><td>Revel</td></tr>
			<tr>
				<td><strong>Final Decision</strong></td>
				<td>Django</td>
			</tr>
			<tr>
				<td><strong>Justifications</strong></td>
				<td>
					<strong>Why not Ruby on Rails?</strong>
					<p>We considered Ruby on Rails as one of our options due to the expressive nature of the ruby language, allowing funtions to be written very fast. Ruby also had a large developer following and library. However, due to scaffolding could mean that ou application is inflexible and also the dynamic nature of Ruby meant that it runs a little slower compares to statically typed languages.</p>
					<strong>Why not Revel</strong>
					<p>Revel was also an option due to its similarity to Ruby on Rails. Revel was written using the Go language which is statically and strongly typed language. Go has strong concurrency and has many multithreading features. However, Revel may not be the most suitable framework due to being too lightweight. This meant that we had to implement a lot features ourselves, making development inefficient.</p>
					<strong>Deciding between Node JS and Django.</strong>
					<p>After some discussion the team agreed that Node JS and Django was the most suitable for this application. However, we it was hard to decide between the two frameworks. Node JS is extremely popular over the last cople of years since the community is large and there is easily to find resources Node JS also shares a common language with web page scripts as Node JS programs are written in Javascript. Node applications are also Event-driven which means it can perform other tasks while wating for asynchronous operations.<br>
					On the other hand, Django is a very high level framework written in python which could lead to rapid development. Django takes care of most aspects of web development such as user authentication and also has an in built admin system. The scalabitlity of Django also makes it very suitable for our application since there are a reasonable amount of users that could potentially use this application.<br>
					Ultimately, the team decided on Django as the framework for the backend as we felt that Django had many in built systems that could be useful to our application, making development the most efficient.</p>
				</td>
			</tr>
		</tbody>
	</table>
</div>

<a href="#top" class="btn btn-primary">^ Back to top</a>

<h3 class="section-header" id="algorithm-research-section">Algorithm Research</h3>
After researching online regarding solutions to the Stable Marriage Problem, we found that applying the **Gale-Shapley Algorithm** would be an effective way to find a stable match between mentors and mentees.

<span class="lead sub-header"><strong>Gale-Shapley Algorithm</strong></span><br>
The Gale-Shapley Algorithm involves a number of iterations or "rounds" where mentees are able to choose a fixed number of prefered mentors ordered by rank. Then the system will match mentors and mentees based on how suitable the match is between a mentor and mentee. By using this algortihm, we can ensure that every mentees gets matched with a mentor and no one is unpaired.

However, since this algorithm is under the assumption that two sets of data are of equal size, in reality the number of mentors and mentees may vary. Hence additional steps had to be implemented in order to overcome problems when there are uneven amount of mentors and mentees. A more detailed design of the implementation of this matching process is available at the Design section. We chose it as it provided the best solution which addressed the stable marriage problem and also ensures that every mentee is matched with a mentor with as much similarity. 

<h3 class="section-header" id="summary-decision-section">Summary of our decisions</h3>
This section is a general summary of the decisions that we have made.

<div class="table-responsive decisionTable"> 
	<table class="table table-bordered">
    	<tbody>
    		<col width="20%">
  			<col width="80%">
  			<tr class="category-header"><td colspan="2">Client Side</td></tr>    		
		    <tr>
		       	<td>Operating platform/environment</td>
		        <td>A hybrid native mobile web application built using AngularJS and Ionic Framework.</td>		        
		    </tr>
		    <tr>
		       	<td>Frontend Framework</td>
		        <td>AngularJS is used to develop our Views and controllers. Various Ionic mobile user interface components were also used for client interaction.</td>		        
		    </tr>
		    <tr class="category-header"><td colspan="2">Server Side</td></tr>
		    <tr>
		       	<td>Django REST Framework</td>
		        <td>We decided to use the Django REST Framework which was written using Python. Django REST Framework has excellent documentation and a very wide development community.</td>
		    </tr>
		    <tr> 
		        <td>Matching Algorithm</td>
		        <td>Gale-Shapley Algorithm</td>
		    </tr>				        
		</tbody>
	</table>
</div>

<a href="#top" class="btn btn-primary">^ Back to top</a>
