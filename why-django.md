Django for web services
=======================


What's Django?
--------------
[Django](https://www.djangoproject.com/) is an open-source web application framework written in Python.


General strengths
-----------------
- It's an actively developed, mature web framework that's not going to go away anytime soon
- There are Python modules to do just about everything, and you can use them in Django apps. Examples include django-auth-ldap which easily hooks into Northwestern's LDAP system


Why it's a good fit for ASG
---------------------------
Django enables rapid development of nontrivial web applications. The trade-off is that it doesn't scale that well. This is fine, because at Northwestern, student-oriented applications will have at most several thousand users. Django should be able to handle this with a few uWSGI threads and if necessary, caching via redis (for sessions) or varnish (for static content apps like guides).


Best practices
--------------
- Use virtualenvs and virtualenvwrapper (with a list of dependencies in a requirements.txt file) to quickly set up projects
- select_related
