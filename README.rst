Cookiecutter Django
=======================

Usage
------

Let's pretend you want to create a Django project called "redditclone". Rather than using ``startproject``
and then editing the results to include your name, email, and various configuration issues that always get forgotten until the worst possible moment, get cookiecutter_ to do all the work.

First, get Cookiecutter. Trust me, it's awesome::

    $ pip install "cookiecutter>=1.4.0"

Now run it against this repo::

    $ cookiecutter https://github.com/soccer99/cookiecutter-django

You'll be prompted for some values. Provide them, then a Django project will be created for you.

**Warning**: After this point, change 'Daniel Greenfeld', 'pydanny', etc to your own information.

Answer the prompts with your own desired options_. For example::

    Cloning into 'cookiecutter-django'...
    remote: Counting objects: 550, done.
    remote: Compressing objects: 100% (310/310), done.
    remote: Total 550 (delta 283), reused 479 (delta 222)
    Receiving objects: 100% (550/550), 127.66 KiB | 58 KiB/s, done.
    Resolving deltas: 100% (283/283), done.
    project_name [Project Name]: Reddit Clone
    project_slug [reddit_clone]: reddit
    author_name [Daniel Roy Greenfeld]: Daniel Greenfeld
    email [you@example.com]: pydanny@gmail.com
    description [A short description of the project.]: A reddit clone.
    domain_name [example.com]: myreddit.com
    version [0.1.0]: 0.0.1
    timezone [UTC]: America/Los_Angeles
    use_whitenoise [n]: n
    use_celery [n]: y
    use_redis [n]: y
    use_rabbitmq [n]: n
    Select postgresql_version:
    1 - 10.3
    2 - 10.2
    3 - 10.1
    4 - 9.6
    5 - 9.5
    6 - 9.4
    7 - 9.3
    Choose from 1, 2, 3, 4 [1]: 1
    keep_local_envs_in_vcs [y]: y
    debug[n]: n

Enter the project and take a look around::

    $ cd reddit/
    $ ls

Create a git repo and push it there::

    $ git init
    $ git add .
    $ git commit -m "first awesome commit"
    $ git remote add origin git@github.com:pydanny/redditclone.git
    $ git push -u origin master

Now take a look at your repo. Don't forget to carefully look at the generated README. Awesome, right?

For local development, see the following:

* `Developing locally`_
* `Developing locally using docker`_

.. _options: http://cookiecutter-django.readthedocs.io/en/latest/project-generation-options.html
.. _`Developing locally`: http://cookiecutter-django.readthedocs.io/en/latest/developing-locally.html
.. _`Developing locally using docker`: http://cookiecutter-django.readthedocs.io/en/latest/developing-locally-docker.html

Community
-----------

* Have questions? **Before you ask questions anywhere else**, please post your question on `Stack Overflow`_ under the *cookiecutter-django* tag. We check there periodically for questions.
* If you think you found a bug or want to request a feature, please open an issue_.
* For anything else, you can chat with us on `Gitter`_.

.. _`Stack Overflow`: http://stackoverflow.com/questions/tagged/cookiecutter-django
.. _`issue`: https://github.com/pydanny/cookiecutter-django/issues
.. _`Gitter`: https://gitter.im/pydanny/cookiecutter-django?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge

For Readers of Two Scoops of Django
--------------------------------------------

You may notice that some elements of this project do not exactly match what we describe in chapter 3. The reason for that is this project, amongst other things, serves as a test bed for trying out new ideas and concepts. Sometimes they work, sometimes they don't, but the end result is that it won't necessarily match precisely what is described in the book I co-authored.

For pyup.io Users
-----------------

If you are using `pyup.io`_ to keep your dependencies updated and secure, use the code *cookiecutter* during checkout to get 15% off every month.

.. _`pyup.io`: https://pyup.io

"Your Stuff"
-------------

Scattered throughout the Python and HTML of this project are places marked with "your stuff". This is where third-party libraries are to be integrated with your project.

Releases
--------

Need a stable release? You can find them at https://github.com/pydanny/cookiecutter-django/releases


Not Exactly What You Want?
---------------------------

This is what I want. *It might not be what you want.* Don't worry, you have options:

Fork This
~~~~~~~~~~

If you have differences in your preferred setup, I encourage you to fork this to create your own version.
Once you have your fork working, let me know and I'll add it to a '*Similar Cookiecutter Templates*' list here.
It's up to you whether or not to rename your fork.

If you do rename your fork, I encourage you to submit it to the following places:

* cookiecutter_ so it gets listed in the README as a template.
* The cookiecutter grid_ on Django Packages.

.. _cookiecutter: https://github.com/audreyr/cookiecutter
.. _grid: https://www.djangopackages.com/grids/g/cookiecutters/

Submit a Pull Request
~~~~~~~~~~~~~~~~~~~~~~

We accept pull requests if they're small, atomic, and make our own project development
experience better.

Articles
---------

* `cookiecutter-django with Nginx, Route 53 and ELB`_ - Feb. 12, 2018
* `cookiecutter-django and Amazon RDS`_ - Feb. 7, 2018
* `Deploying Cookiecutter-Django with Docker-Compose`_ - Oct. 19, 2017
* `Using Cookiecutter to Jumpstart a Django Project on Windows with PyCharm`_ - May 19, 2017
* `Exploring with Cookiecutter`_ - Dec. 3, 2016
* `Introduction to Cookiecutter-Django`_ - Feb. 19, 2016
* `Django and GitLab - Running Continuous Integration and tests with your FREE account`_ - May. 11, 2016
* `Development and Deployment of Cookiecutter-Django on Fedora`_ - Jan. 18, 2016
* `Development and Deployment of Cookiecutter-Django via Docker`_ - Dec. 29, 2015
* `How to create a Django Application using Cookiecutter and Django 1.8`_ - Sept. 12, 2015

Have a blog or online publication? Write about your cookiecutter-django tips and tricks, then send us a pull request with the link.

.. _`cookiecutter-django with Nginx, Route 53 and ELB`: https://msaizar.com/blog/cookiecutter-django-nginx-route-53-and-elb/
.. _`cookiecutter-django and Amazon RDS`: https://msaizar.com/blog/cookiecutter-django-and-amazon-rds/
.. _`Deploying Cookiecutter-Django with Docker-Compose`: http://adamantine.me/2017/10/19/deploying-cookiecutter-django-with-docker-compose/
.. _`Exploring with Cookiecutter`: http://www.snowboardingcoder.com/django/2016/12/03/exploring-with-cookiecutter/
.. _`Using Cookiecutter to Jumpstart a Django Project on Windows with PyCharm`: https://joshuahunter.com/posts/using-cookiecutter-to-jumpstart-a-django-project-on-windows-with-pycharm/

.. _`Development and Deployment of Cookiecutter-Django via Docker`: https://realpython.com/blog/python/development-and-deployment-of-cookiecutter-django-via-docker/
.. _`Development and Deployment of Cookiecutter-Django on Fedora`: https://realpython.com/blog/python/development-and-deployment-of-cookiecutter-django-on-fedora/
.. _`How to create a Django Application using Cookiecutter and Django 1.8`: https://www.swapps.io/blog/how-to-create-a-django-application-using-cookiecutter-and-django-1-8/
.. _`Introduction to Cookiecutter-Django`: http://krzysztofzuraw.com/blog/2016/django-cookiecutter.html
.. _`Django and GitLab - Running Continuous Integration and tests with your FREE account`: http://dezoito.github.io/2016/05/11/django-gitlab-continuous-integration-phantomjs.html

Code of Conduct
---------------

Everyone interacting in the Cookiecutter project's codebases, issue trackers, chat
rooms, and mailing lists is expected to follow the `PyPA Code of Conduct`_.


.. _`PyPA Code of Conduct`: https://www.pypa.io/en/latest/code-of-conduct/
