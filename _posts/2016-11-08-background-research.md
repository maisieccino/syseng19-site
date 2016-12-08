---
layout: post
title:  "Background Research"
date:   2016-11-05 00:30:51 +0100
categories: development
---

<h3 class="section-header">Overcoming the Stable Marriage Problem</h3>
After researching online regarding solutions to the Stable Marriage Problem, we found that applying the **Gale-Shapley Algorithm** would be an effective way to find a stable match between mentors and mentees.

The Gale-Shapley Algorithm involves a number of iterations or "rounds" where mentees are able to choose a fixed number of prefered mentors ordered by rank. Then the system will match mentors and mentees based on how suitable the match is between a mentor and mentee. By using this algortihm, we can ensure that every mentees gets matched with a mentor and no one is unpaired. A more detailed design of thhe matching process is available at the Architecture Research and Design section.

__MORE__

<h3 class="section-header">Existing Solutions</h3>
We searched for some existing applications that does matching between individuals as part of the initial stages of research. This helped us gain a basic idea of some features that we may like to include in our final product.

<span class="lead sub-header">Mentor Match</span><br>
**Mentor Match** is an existing open source website that had a very similar concept to what our client was trying to acheive. Mentor Match is open to everyone and allows individuals with experience in a particular skillset to act as mentors to help mentees improve on that particular skillset.
Since this website is open to everyone, it makes exchange of knowledge very simple as anyone could take part in it. 

However, there are certain features that the website lacks in terms of security as there is no verification as there is no way to assure that users applying to be a mentor has the skillset to become one. Also there were different types of mentor schemes requested by our client which differ with the schemes provided on the Mentor Match website. Despite the differences in structure of this website with the web application we are about to build, Mentor Match could be a useful guideline on the basic foundation of our web application.

<span class="lead sub-header">Business Mentoring</span><br>
Matching based on:
1. Focus areas/ competencies: There system have 25 default competencies to choose. (useful)
2. Forced choice questions:Provide questions that have several answers to select. Make the preferences of matching more specific. (useful)
3. Personality test:(optional)
4. Ranking of key roles: In this section, mentorees must decide what type of mentor they want based on how they order the following roles: teacher, sponsor, cheerleader, counselor, and friend (meaning if they put "cheerleader" first and "counselor" last, it's more important that the mentor is a cheerleader than a friend). Mentors must decide the type of mentor they want to be and do the same thing, ranking the roles in order of most important to least. (useful)
5. Essay section (not useful)

They also provide system matching:
1. Auto matching: makes matches based on algorithm without any review. 
2. three-steps-matching (also combines human touch, not 100% system matching): 
   * Program manager choose 3 tentative mentors for individual mentee.
   * Comparing mentoring forms(inforamtion) of the mentee with each mentor
   * The program manager makes the final choice

What we could learn from this project:
As the result of precise matching algorithm,this application has high percentage of successful matching (90% according to its website). From my research, the division of focus areas and ranking of key roles play an important role in matching, thats what we could follow in our app, give a list of skills as tags for user to choose. 

<span class="lead sub-header">Dating Applications</span><br>
Dating applications may not be the most professional apps to be used in a workplace, however the concept of these types of application is very similar to what was requested by our client. Our Client even quoted that this application "could be considered a kind of dating app". Most dating applications have simple and elegent user interfaces that users can act easily with. This could be applied to our application so that employees in Atos workplace can use our application with ease. Concepts such as user profiles, notifications, instant messaging could be included in our application which already exist in dating applications. 