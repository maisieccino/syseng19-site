---
layout: post
title:  "Background Research"
date:   2016-11-05 00:30:51 +0100
categories: development
---

<h3 class="section-header">Overcoming the Stable Marriage Problem</h3>
After researching online regarding solutions to the Stable Marriage Problem, we found that applying the **Gale-Shapley Algorithm** would be an effective way to find a stable match between mentors and mentees.

The Gale-Shapley Algorithm involves a number of iterations or "rounds" where mentees are able to choose a fixed number of prefered mentors ordered by rank. Then the system will match mentors and mentees based on how suitable the match is between a mentor and mentee. By using this algortihm, we can ensure that every mentees gets matched with a mentor and no one is unpaired. A more detailed design of thhe matching process is available at the Architecture Research and Design section.

<h3 class="section-header">Existing Solutions</h3>
We searched for some existing applications that does matching between individuals as part of the initial stages of research. This helped us gain a basic idea of some features that we may like to include in our final product.

<span class="lead" style="font-size:20px;">Mentor Match</span><br>
**Mentor Match** is an existing open source website that had a very similar concept to what our client was trying to acheive. Mentor Match is open to everyone and allows individuals with experience in a particular skillset to act as mentors to help mentees improve on that particular skillset. 

Since this website is open to everyone, it makes exchange of knowledge very simple as anyone could take part in it. However, there are certain features that the website lacks in terms of security as there is no verification when applying to become a mentor