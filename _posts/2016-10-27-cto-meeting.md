---
layout: post
title:  "CTO Meeting 1 Notes"
date:   2016-10-10 14:00:00 +0100
categories: meetings
attendees: [ 'Chris','Matt','Harry','Mike Smith' ]
---

This meeting involved us talking to Mike Smith, CTO of Atos, about the technical constraints of the project.

* Use what we're most familiar with
* looking for _ideas_ not the final system necessarily (although it's a challenge!)
* they're not able to provide infrastructure
* ask department for a VPS (done!)
* may be a different no of pairs (i.e. more mentees than mentors)
* may be times when a mentee has no mentor and has to miss out
* natural language processing would be pretty cool
* unlikely to use corporate DB - privacy reasons etc
* list things that might be important
* work out primary considerations (for matching)
* score matches? (i.e. out of 100)

User story
----------
* individual registers on system
* registers for mentor position or mentee position
* add details
* processing step
* then.. shortlist?
* recommendation?
* preferences?
* match made?
* where does the final decision rest?
* will there be a "cooling-off" period where mentees can change their minds?
* "think about design"
* relationship object separate from user object
* "status" object
* admin view "very useful"
* how will we report status? rating out of 5stars? text?
* authentication:
  - Atos have their own SSO
  - Don't waste time writing our own
  - Use Twitter/Facebook login, or OAuth
  - Modular is good so that it can integrate
* Branding guidelines
  - no hard guidelines
  - don't worry about this too much.
* Catch up with Jane...?
  - book every 2-4 weeks?
* No restrictions on code
  - we apparently have IP on our work..?
  - Atos has permission to use our work if they like it though.
  - They're happy for us to make the repo public.
