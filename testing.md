---
layout: page
title: "Testing"
permalink: /testing/
navigation: true
order: 7
---

Our Testing Methodology
===
The way we tested our system varied considerably between the webapp 
and the API server. The development of the API largely followed a
Behaviour-Driven Development (BDD), which aligned well with the way
that our project was organised. The webapp, by its nature, is a lot
more difficult to unit test and thus we adopted an iterative process,
where a feature was developed and the developer used black-box testing
to make sure the feature worked.

API Testing
===

Automated Testing Suite
---
Because the API was developed using the Django framework, we were
able to use its own testing harness and mocking environment. This test
environment can create a test database on the fly, and mock web requests
if we so wish to automate testing of the real API endpoints without having
to power up an actual web server. In addition to this, the test harness
automatically bundled each test in a test case into a single database
transaction by default, meaning that the suite ran much faster than it
would otherwise.

There were three main types of test in the automated suite: model tests,
serializer tests, and API tests. The model tests acted like traditional
unit tests, which tested model methods to ensure that they returned the
correct value for a range of different inputs. The serializer tests
were used to make sure that user input was properly validated and that
the data serializers did not leak any private information (for instance,
passwords). Finally, the API tests mocked API calls to the server, to make
sure that the server could return the correct response code and data for a
range of scenarios. These tests were developed according to the API
specification, to make sure that the error codes were what an API consumer
would expect to receive.

Continuous Integration (CI)
---
Thanks to these automated tests, we were able to set up a continuous
integration solution to ensure that new code did not break the existing
system. We chose Travis CI, because of its simple integration with
GitHub, where our code repository is stored. We configured Travis to
run the test suite as part of its test script, and set it up so that
tests would run on all commits and pull requests. We also modified the
GitHub repository settings so that code could not be pushed straight to
the master branch (all code had to be merged in via pull request), and
pull requests could not be merged into master unless the CI build passed.

Finally, to take this even further, we hooked up our CI system to the
development server, meaning that once code passed tests on the master
branch, a script would be run that deploys the code to our server,
performs any package installs and database migrations, then restarts
the server so that it's running on the new code. This ties in partly
with the 'dogfooding' methodology that's used on the web app development.
You can view all of our CI builds on the link below.

[View Our Travis CI Builds](travis-ci.org/mbellgb/syseng19-code/) 

Manual Black-Box Testing
---
Often, to ensure our tests were working correctly, we'd perform manual
black-box testing. This would involve making API calls in the same manner
as a real API consumer, and check that the output received was what was
expected. For this, we normally used the Postman app, or cURL. Using
Postman, we could simulate the entire authentication flow, and test
actions like signing up for mentorship programmes.

Web App Testing
===

User Acceptance Testing
---
(add something here)

Onboard Hardware Testing
---
(Explain how you tested on real devices etc)
