Session 5 - Utilities and Modules
=================================

Today we will carry on the work with modules and more specific the 3rd party module BeautifulSoup for webscrabing. You will also work with persitance in your docker containers, meaning how you will "save" your installed modules done by pip install.

Learning goals
--------------
After this week you will be able to:
       
        - Use python build in modules.
        - Find and use 3rd party modules.
        - Save and Share your modules installed in a docker container.   
        - work with markdown documents.
        - Work with the module BeautifullSoup for webscrabing.


Materials
---------
* `Slides <_static/notes_docker_requirements_webscrabing.slides.html>`_  `(Notebook) <notebooks/notes_docker_requirements_webscrabing.ipynb>`_
* `Beautiful Soup Documentation <https://www.crummy.com/software/BeautifulSoup/bs4/doc/>`_
* `Html to markdown <notebooks/html_markdown.rst>`_
* `Docker Commands <cheatsheet.rst#week-38-utilities-and-modules>`_
* `Code examples from today <https://github.com/python-elective-kea/spring2021-code-examples-from-teachings/tree/master/ses5>`_

Exercises
---------
------
Docker
------

Ex 1: Clone, build and run
**************************

* Clone this repository:
  
  * git clone https://github.com/python-elective-kea/clbo-alpine-dev-env.git

* Build an Image based on the repositorys Dockerfile.
  
  * docker build --tag clbo/python

* Run a container based on this image
  
  * docker run -it --rm -v ${PWD}:/docs clbo/python

        
Ex 2: Node app and docker
*************************

* `Build and run your image <https://docs.docker.com/get-started/part2/>`_

Ex 3: Create and run a 'Hello world' C application
***************************************************

`Solution <exercises/solution/04_modules/solutions.rst>`_

Based on this docker image: https://hub.docker.com/_/gcc create and run a Hello World app, written i the C language.

The code you need is something like this:

.. code::
   
   #include <stdio.h>
   int main() {
       // printf() displays the string inside quotation
       printf("Hello, World!");
       return 0;
   } 
   

Ex 4: Docker'ise' your own projects
***********************************

This exercise should be done in groups.
* You should create a project that makes use of the requests module.
* You should push this project to a github account and all in the group should have push rights to this repository.
* The project should contain a Dockerfile that as a minimum has a :code:`pip install -r requirements.txt` line in it.
* All group members should clone the repository, build the image based on the Dockerfile, and run a container with the right modules installed.

When this setup is up and running each group member should: 

* install a new 3rd. party module in the container. 
* Create some simple (maybe even stupid) code that makes use of this module
* do a :code:`pip freeze > requirements.txt`
* Push the changes to github
* Pull the other group members changes and do a :code:`docker build --tag nameoftheimage:1.1 .`  

.. warning::
        It might be a good idea that each group member does this one at a time.

------
Python
------

Ex 5: Build a Web Scraper With Python
*************************************

`Solution <exercises/solution/04_modules/solutions.rst>`_

1. `Build a Web Scraper With Python <https://realpython.com/beautiful-soup-web-scraper-python/>`_
2. Find all relevant python jobs on this website: `jobnet.dk <https://job.jobnet.dk/CV>`_ or `jobindex.dk <https://www.jobindex.dk/?lang=dk>`_


Ex 6: Simple scraber with requests (and BS)
*******************************************

Do the `Ex 7: Simple scraber with requests <week37.rst#ex-7-simple-scraber-with-requests>`_ exercise from last week but now also by using the BeautifullSoup module.


Ex 7: From Html to Markdown
***************************

Get the html of this `page <https://clbokea.github.io/exam/assignment_2.html>`_ , and change it from a html page to a Markdown page. 

You can read a bit about markdown `here <notebooks/html_markdown.rst>`_
