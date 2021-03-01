Session 6 - OOP
===============

.. note:: Homework
   
   Before this class you should have read and understood this text `Object-Oriented Programming (OOP) in Python 3 <https://realpython.com/python3-object-oriented-programming/>`_. These are basic OOP concepts, which you have already woorked with in the forst part of your education. You just need to be up to date with how this is done, and how the syntax is done in python.

Today we will work with the basics of Object oriented programming in python. 

Learning goals
--------------
After having worked with these topics you will be able to:
      
   - create Classes, Objects, instance and class variables, methods and initializer methods. 
   - make use of single and multiple inheritance.   
   - explain when and why to use classes and objects instead of procedural style. 
   - relate the pythonic OOP style to other languages  (Java e.g) 

Materials
---------
* `Object-Oriented Programming (OOP) in Python 3 <https://realpython.com/python3-object-oriented-programming/>`_
* `Python args and kwargs: Demystified <https://realpython.com/python-kwargs-and-args/>`_
* `Notebook on classes <notebooks/class_notes.ipynb>`_
* `Code examples from teachings <https://github.com/python-elective-kea/spring2021-code-examples-from-teachings/tree/master/ses6>`_

.. * `Video on when not to use classes <>`_
        * Article on when to and not to use classes.
        * Example on classes with 2 methods, and one is __init__
        * Refactor example into a function instead


Exercises
---------


.. raw:: html
   
   <hr>


-------------------
EX 1: Bank Exercise 
-------------------

`Solution <exercises/solution/04_oop/solution.rst>`_

Create a Bank, an Account, and a Customer class.

* All classes should be in a single file. 
* The bank class should be able to hold many account.
* You should be able to add new accounts.
* The Account class should have relevant details.
* The Customer class Should also have relevant details.

Stick to the techniques we have covered so far.

* Add the abillity for you __init__ method to handle different inputs (parameters).


.. raw:: html
   
   <hr>



----------------
Ex 2: Angry Bird
----------------

`Solution <exercises/solution/04_oop/solution.rst>`_

In this exercises you are going to create a simple terminal version of this `Angry Bird online coding teaching tool for kids <https://studio.code.org/hoc/1>`_ .

.. image:: _static/angry_bird.png

You should make this as an OOP application, and your classes could be like this. 

**Bird**

Should know its *current position*, and should know in what *direction* it is moving. It should be able to *move forward*, *turn left*, and *turn right*.
It should also have an action invoked when it looses the game, and one when it wins. 


**Pig**

Should know its *position*. 
It should also have an action invoked when it looses the game, and one when it wins. 

**Board**

Should initialize a Bird and a Pig object. It should *display* the board with the bird and the pig in starting positions. It should have a *run method*

.. code::

        *  *  *  *  *  *  *  *  *  *
        *  *  *  *  *  *  *  *  *  *
        *  *  B  *  *  *  *  *  *  *
        *  *  *  *  *  *  *  *  *  *
        *  *  *  *  *  *  *  *  *  *
        *  *  *  *  *  *  *  *  *  *
        *  *  *  *  *  *  *  *  *  *
        *  *  *  *  *  *  P  *  *  *
        *  *  *  *  *  *  *  *  *  *
        *  *  *  *  *  *  *  *  *  *


**Workspace**

Should have a display method printing out instructions on what to do. It should have a method being responsible of creating a collection of commands from user input. 


**Game**

This class is responsible of running the application. It should create objects of Board and Workspace and call their display methods. It should also be responsible for deciding if the bird hit the pig or not. 

**********
Screencast
**********

You can see a prototype of this exercise here. You are of cause welcome to improve the game, but this could be a solution. 

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/n9Ths1CSCkU" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

