Session 9 - Functions &  Decorators  
===================================

Decorators in python are widely used to add new functionallity to already existing code.

You have already used decorators in your code. A :code:`@property` is an example of this. Here you anotate a method with 'something' to make it able to do 'more' than the method in it self can do. 

You also know the concept from the Spring Framework you worked with previous in your education. Here you would add some more functionality (more code) to your already existing code by anotating it with :code:`@Controler` or :code:`@Autowired`. In both cases you add extra code to your code and get some new functionality.     . 

:code:`@property` is a python build in decorator, but today you will be making your own decorators.

The boilerplate syntax of a decorator is like this:

.. code:: python 
   :linenos:

   def decorator(func):
       def wrapper_decorator(*args, **kwargs):
               # Do something before
               value = func(*args, **kwargs) // execute function
               # Do something after
               return value
       
       return wrapper_decorator

And if you want to use it you will do like so:

.. code:: python
   :linenos:

   @decorator
   def greet(name):
        return 'Hello ' + name

We will start out by using a new editor, Jupyter Notebook.

Learning goals
--------------
By reading the texts in the materials section, doing the 3 exercises, and follow the teachings, you will be able to explain what a decorator is, when to use it, and how the inner parts of a decorator function is made up, and you will be able to create your own, and use others already made decorators. 

After this week you will know about:

        - First class functions 
        - Inner functions
        - Decorator functions

You will futhermore be able to install and use a Jupyter Notebook.

Materials
---------
* `Getting started with Jupyter Notebook <notebooks/jupyter_notebook.md>`_
* `Getting Started With Jupyter Notebook for Python <https://medium.com/codingthesmartway-com-blog/getting-started-with-jupyter-notebook-for-python-4e7082bd5d46>`_  (skip the install part since we do it through docker)
* `Primer on Python Decorators <https://realpython.com/primer-on-python-decorators/>`_
* `Python Inner Functions—What Are They Good For? <https://realpython.com/inner-functions-what-are-they-good-for/>`_
* `Notebook on Decorators <notebooks/Decorators.ipynb>`_
* `Code examples from teachings <https://github.com/python-elective-kea/spring2021-code-examples-from-teachings/tree/master/ses9>`_


Exercises
---------
* :ref:`Small exercises <exsm>`
* :ref:`Ex1: Time it <ex1>`
* :ref:`Ex2: memory-profiler <ex2>`
* :ref:`Ex3: Slow down code <ex3>`

.. _exsm:

---------------
Small Exercises
---------------

`Solution <exercises/solution/08_decorators/solutions.rst>`_

With this function as a starting point 

.. code:: python
   :linenos:

   def add(*args):
        sum = 0     
        for i in args:
            sum += i          
       return sum 

1. Write a decorator that writes to a log file the time stamp of each time this function is called.
2. Change the log decorator to also printing the values of the argument together with the timestamp.
3. Print the result of the decorated function to the log file also. 
4. Create a new function and call it printer(text) that takes a text as parameter and either returns or prints the text 2 times. Decorate it with your logfunction. Does it work?    




.. _ex1:  

-------------
Ex1: Time it!
-------------

`Solution <exercises/solution/08_decorators/solutions.rst>`_

Next week we will work with *generators*, *generator expressions* and *list comprehensions*. These topics has a lot to do with program efficiency. 

For this we will be measuring our code in diffenrent ways and especialy we will *'time it'* and *'messure memmory usage'*. 

If you want to messure how much time it takes to execute a piece of code you could do the followin:

.. code:: python
   :linenos:

   import time

   start = time.time()
   // do some stuff you want to meassure here
   end = time.time()
   print(end - start)

   
Instead of writing this every time you need to time something, you could write a docorator function that does the job for you. 

**Task:**

Your job is, to write a decorator function that can time any piece of code.

You can read about time by starting your interpretor and write:

.. code:: python

   > import time
   > help(time)



   
.. _ex2:

--------------------
Ex2: memory-profiler 
--------------------

Measuring the memory ussage of an object, function or piece of code can be of equally importance as the timing functionallity you just created.

Python has a build in module called :code:`resource`. This is a unix system only module. Luckily we are all on a unix based system when we use docker for python development. 


**Task:**

Your job is, to write a decorator function that can messure the memory usage of any piece of code.


.. _ex3: 

-------------------
Ex3: Slow down code
------------------- 

`Solution <exercises/solution/08_decorators/solutions.rst>`_

The code below counts down from n -> 0. So calling countdown(5) prints: 5 4 3 2 1 Liftoff!

.. code:: python
   :linenos:

   def countdown(n):
        if not n:   # 0 is false, not false is true
            return n
        else:
            print(n, end=' ')
            return countdown(n-1) # call the same function with n as one less 


(The function is a recursive function, which you might or might not have worked with before.)

**Task:**

Create a decorator function that slows down your code by 1 second for each step. Call this function *slowdown()*


For this you should  use the 'time' module.
                        
When you got the 'slowdown code' working on this recursive function, try to create a more (for you) normal function that does the countdown using a loop, and see what happens if you decorate that function with you slowdown() function.







