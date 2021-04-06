Commandline Cheatsheet
======================
In this cheatsheet you will find important and hard to remember terminal commands.

Docker Commands
---------------

---------------------------------
Session 1 - Introduction to python 
---------------------------------

.. code::
   
   $ docker run -it --rm ubuntu  // creates and runs a simple ubuntu container with interactive access and removal after use. 
   $ docker run -it --rm python bash // same as above, but now a python image. starts in a bash terminal.
   $ docker run -it --rm -v ${PWD}:/docs python bash  // same as above, but now sharing files from the current directory to/from /docs folder in the container.
 

---------------------------------
Session 5 - Utilities and Modules
---------------------------------

.. code::

        $ docker build --tag webscrabing:latest .
        $ docker run -it --rm -v ${PWD}:/docs webscrabing 

----------------------------------
Session 9 - Functions & Decorators
----------------------------------

.. code::

        $ docker run --rm -p 8888:8888 -v ${PWD}:/home/jovyan/work jupyter/datascience-notebook 


---------------
Sphinx commands
---------------

.. code::
   
   $ docker run --rm -v ${PWD}:/docs sphinx /bin/sh -c 'cd sphinx/; make html'


-----
Links
-----

* `How to Create a Docker Image From a Container <https://www.scalyr.com/blog/create-docker-image/>`_





