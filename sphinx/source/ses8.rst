Session 8 - The python datamodel
================================

Today we will look at the python data model. 

After this you will be able to implement code in own classes that allow you to use python built-in functions to interact with these object.

**Example:**

If you want to be able to use the build in function :code:`len()` on your object you should implement the :code:`__len__` method in your class.  

If you want to be able to use the :code:`==` operator on your object you should implement the :code:`__eq__` method in your class. 

If you want to be able to use the :code:`in` key word on your object you should implement the :code:`__contains__` method in your class. 


Learning goals
--------------

    * Create your own classes, that behave like any other Python Object, and are able to interact with pythons build in functions. 
     
Materials
---------

* `A Guide to Python's Magic Methods <https://rszalski.github.io/magicmethods/>`_
* `Notebook on Datamodel <notebooks/OOP_Encapsulation_Propeties.ipynb#Datamodel>`_
* `Code examples from teachings <https://github.com/python-elective-kea/spring2021-code-examples-from-teachings/tree/master/ses8>`_

Exercises
---------

------------------
Ex1: Deck of cards
------------------

`Solution <exercises/solution/06_datamodel/solutions.rst>`_

Continue with the deck example and implement the 

* :code:`__len__` method
* :code:`__add__` method
* :code:`__repr__` method
* :code:`__str__` method
* :code:`__setitem__` method
* :code:`__delitem__` method

We look at this together in a short while.

When you a done, take a look at the 2 exercises below and ask your questions when we meet. 


.. raw:: html
   
   <hr>

* `Linked List <exercises/protocol_linked_list.rst>`_  
* `Jelly Beans <exercises/JellyBeans.rst>`_ 
