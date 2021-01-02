Week 40 - Encapsulation
=======================

The pythonic approach starts out with the quite bold statement that all attributes are public, and unless specificly needed there are not any reason to make them anything else but public. If you think on back on your java development times, it is in reality seldome that you do some coding tasks that could not have been done with public attributes instead of privates with connected getters and setters. The pythonic approach to this problem is: make everything public, and if at some point you need to encapsulate, decorate your attributes and change it into a property. Today we will work with this approach in mind.  

Learning goals
--------------
After this week you will be able to:
        
- Understand the pythonic approach to encapsulation. 
- Use private and public attributes in your code
- Explain what is meant by private in python 
- Work with properties to use encapsulation.
- And explain the pros and cons of properties and public attributes compared to Java´s private attributes with getters and setters. 

Materials
---------
* `Properties vs. Getters and Setters <https://www.python-course.eu/python3_properties.php>`_
* `Private attributes and methods <https://www.bogotobogo.com/python/python_private_attributes_methods.php>`_
* `Notebook on properties <notebooks/OOP_Encapsulation_Propeties.rst>`_
* `Code examples from teachings <https://github.com/python-elective-kea/fall2020-code-examples-from-teachings/tree/master/w40>`_


Exercises
---------

------------------------------------
Encaptiolation & Propeties exercises
------------------------------------

All following exercises should be done by using **Properties** when needed. The focus should be on encapsulation. 


Ex 1:  Car object
*****************

`Solution <exercises/solution/05_encapsulation/solutions.rst>`_

Create a Car class. When instanciated the object should be able to take 4 attributes (Make, Model, bhp, mph). They all 4 should be properties.



Ex 2: Bank
**********

`Solution <exercises/solution/05_encapsulation/solutions.rst>`_

In the exercise from last monday with the bank, account and customer, change the code to use properties instead of the public variables.  

.. code:: python
   :linenos:

   class Bank:    
        def __init__(self):
           self.accounts = []

   class Account:
        def __init__(self, no, cust):
           self.no = no
           self.cust = cust

   class Customer:
        def __init__(self, name):
           self.name = name


* The bank class should futher be change into not taking any accounts as parameters at initialization. 
* The accouts should be added afterwards, eithers as a single account one at a time, or as a collection of accounts (many at the sametime).      
* Somewhere you should change the code so that a customer only can create one account.     
* The Customer class should make sure that the customer is over 18 year of age.





Ex 3: Machine -> printer
************************

`Solution <exercises/solution/05_encapsulation/solutions.rst>`_


* Create a Machine class that takes care of powering on and off a the machine.   
* Create a printer class that is a subclass of the Machine super class.   
* The printer should be able to print to console.  
* The printer should have a papertray, which should be in its own class. The papertray class should keep track of the paper, it should have the abillity to use paper and load new paper in the tray if empty.  


