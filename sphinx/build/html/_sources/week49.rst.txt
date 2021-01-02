Week 49 - Python tips & Tricks
==============================
Todays topic are actually topics. We will cover a lot of small usefull python features that for most cases can speed up the development time. 

Learning Goals
--------------
After this week you will be able to:

* Understand pythons contextlib functionallity
* Turn a docker container into a webserver on a local network. 


Materials
---------
* `Notebook on Tips & Tricks <notebooks/Tips_Tricks.ipynb>`_

Exercises
---------

---------------------------
Ex 1: Menu and dictionaries 
---------------------------

In the module below, you should create a register dictionary that has the name of each function as a key and the function itself as a value.   

{'home' : home, 'about' : about}

The register should always corospond to the functions that are in the file.

It would be a good idea to use a decorator for this task. (but be aware that it might be a bit more simple than the decorators we worked with 2 weeks ago)

.. code:: python
   :linenos:

   register = {}
   def home():
        return 'I am the Home page'
   def about():
        return 'I am the About page'
   def contact():
        return 'I am the Contact page'

2. You should simulate a website menu that in a loop asks you what page you want to see and gives you the return value of the functions.

3. Add a menu point called exit. This element should exit the loop.

--------------------------------------------
Ex 2: Serve a Flask website on local network
--------------------------------------------
Based on this app.py file:
   
.. code:: python 
   :linenos:

   from flask import Flask
   app = Flask(__name__)

   @app.route('/')
   def hello_world():
       return 'Hello, World!'

Create a docker container that runs and serves the website on a local network. (You should be able to see the website in your phones browser)

You can read more about Flask in this `Quickstart Guide <https://flask.palletsprojects.com/en/1.1.x/quickstart/>`_

