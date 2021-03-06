FAQ
====

.. index:: FAQ, 12-Factor App

Why is there a django.contrib.sites directory in cookiecutter-django?
---------------------------------------------------------------------

It is there to add a migration so you don't have to manually change the ``sites.Site`` record from ``example.com`` to whatever your domain is. Instead, your ``{{cookiecutter.domain_name}}`` and {{cookiecutter.project_name}} value is placed by **Cookiecutter** in the domain and name fields respectively.

See `0002_set_site_domain_and_name.py`_.

.. _`0002_set_site_domain_and_name.py`: https://github.com/pydanny/cookiecutter-django/blob/master/%7B%7Bcookiecutter.repo_name%7D%7D/%7B%7Bcookiecutter.repo_name%7D%7D/contrib/sites/migrations/0002_set_site_domain_and_name.py


Why aren't you using just one configuration file (12-Factor App)
----------------------------------------------------------------------

TODO

Why doesn't this follow the layout from Two Scoops of Django 1.8?
----------------------------------------------------------------------

You may notice that some elements of this project do not exactly match what we describe in chapter 3 of `Two Scoops of Django`_. The reason for that is this project, amongst other things, serves as a test bed for trying out new ideas and concepts. Sometimes they work, sometimes they don't, but the end result is that it won't necessarily match precisely what is described in the book I co-authored.


.. _`Two Scoops of Django`: http://twoscoopspress.com/products/two-scoops-of-django-1-8
