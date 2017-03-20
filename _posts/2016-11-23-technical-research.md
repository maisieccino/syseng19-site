---
layout: post
title:  "Technical Research"
date:   2016-11-20 00:30:51 +0100
categories: research
---


This page details all the technical research we have done (excluding architecture) throughout this project, including open-source libraries and frameworks that could be useful for the final system. Our research was split in to 2 categories which was frontend research and backend research.

__MORE__

<a href="#back-end" style="margin-top: 7px;" class="btn btn-primary">1. Backend Frameworks/Libraries</a>
<a href="#front-end" style="margin-top: 7px;" class="btn btn-primary">2. Frontend Frameworks/Libraries</a>

<h3 id="back-end" class="section-header">Backend Frameworks/Libraries</h3>

<!-- Node.js -->
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

<h3 id="front-end" class="section-header">Frontend Frameworks/Libraries</h3>

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


