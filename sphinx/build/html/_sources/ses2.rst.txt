Session 2 - Data Structures: List & Tuples
==========================================

Today we will work with data structures in python. You will by the end of these sessions be able to use Lists and Tuples, read and Write to Files and work with the for and while loop.

Learning goals
--------------

After this week you will be able to:
        
        - Work with lists, tuples
        - Loop over sequences with a for, foreach & while loops.  
        - Sort sequences using the build in sorted function and use its key parameter to perform custom sorting.  
        - Read from files and write to files using the build in "open" function. 

Materials
---------

* `Lists and Tuples in Python <https://realpython.com/python-lists-tuples/>`_
* `Tuples in Python <https://www.datacamp.com/community/tutorials/python-tuples>`_
* `Python "for" Loops <https://realpython.com/python-for-loop/>`_
* `Python "while" Loops <https://realpython.com/python-while-loop/>`_
* `How to Use sorted() and sort() in Python <https://realpython.com/python-sort/>`_
* `Slides <_static/noterlists_tuples.slides.html>`_  `(notebook) <notebooks/noterlists_tuples.ipynb>`_
* `Code examples and videos from teachings <https://github.com/python-elective-kea/spring2021-code-examples-from-teachings/tree/master/ses2>`_
* `How to Learn Python in Five Minutes <https://www.youtube.com/watch?v=ohr6O78jGzs>`_

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/ohr6O78jGzs" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Exercises
---------
---------------
Ex 0.1: Slicing
---------------

`Solution <exercises/solution/02_lists/sorted_exercises.rst>`_

By using the slicing syntax change the following collections.

After slicing:

.. code:: Python
        :linenos:

        ['Hello', 'World', 'Huston', 'we', 'are', 'here'] should become -> ['World', 'Huston', 'we', 'are']
        ['Hello', 'World', 'Huston', 'we', 'are', 'here'] -> ['Hello', 'World']
        ['Hello', 'World', 'Huston', 'we', 'are', 'here'] -> ['are', 'here']
        ['Hello', 'World', 'Huston', 'we', 'are', 'here'] -> ['are']
        ['Hello', 'World', 'Huston', 'we', 'are', 'here'] -> ['Hello', 'Huston', 'are']
        ['Hello', 'World', 'Huston', 'we', 'are', 'here'] -> ['here', 'are', 'we', 'Huston', 'World', 'Hello']
        ('Hello', 'World', 'Huston', 'we', 'are', 'here') should become -> ['World', 'Huston', 'we', 'are']
        'Hello World Huston we are here' -> 'World Huston we'

Figure out more on your own and practice this a lot!    

---------------------------------
Ex 1: Build-in functions on lists
---------------------------------

| Look at this list of pythons `build in functions <https://docs.python.org/3/library/functions.html>`_.
| Try all of these in the interpretor (on a list you create). e.g  :code:`len(a)`   
| Not all will work on lists, but try it out and see what works. 


-----------------
Ex 2: Sort a Text
-----------------

`Solution <exercises/solution/02_lists/sorted_exercises.rst>`_

1. Create a function that takes a string as a parameter and returns a list.
2. The function should remove all vowels and sort the consonants in alphabetic order, and the return the result.


-----------------
Ex 3: Sort a list
-----------------
`Solution <exercises/solution/02_lists/sorted_exercises.rst>`_

1. Create a list of strings with names in it. (l = ['Claus', 'Ib', 'Per'])
2. Sort this list by using the sorted() build in function.
3. Sort the list in reversed order. 
4. Sort the list on the lenght of the name.
5. Sort the list based on the last letter in the name.
6. Sort the list with the names where the letter 'a' is in the name first.

-----------
Ex 4: Files
-----------

`Solution <exercises/solution/02_lists/sorted_exercises.rst>`_

1. Create a file and call it lyrics.txt (it does not need to have any content)
2. Create a new file and call it songs.docx and in this file write 3 lines of text to it.
3. open and read the content and write it to your terminal window.
   * you should use both the read(), readline(), and readlines() methods for this. (so 3 times the same output).

---------------------------
Ex 5: Sort a list of tuples
---------------------------

`Solution <exercises/solution/02_lists/sorted_exercises.rst>`_

1. Based on this list of tuples:     
:code:`[(1,2),(2,2),(3,2),(2,1),(2,2),(1,5), (10,4), (10, 1), (3, 1)]`    

2. Sort the list so the result looks like this:  
:code:`[(2, 1), (3, 1), (10, 1), (1, 2), (2, 2), (2, 2), (3, 2), (10, 4), (1, 5)]`   

.. note:: 
        
        | This is first sorted by the last element in the tuple and then the first element in the tuple.
        | You should do this in 1 step, but it might help you to try it out in 2 steps first. 


-----------------------
List & Tuples exercises
-----------------------
`Solution <exercises/solution/02_lists/sorted_exercises.rst>`_

* `List & tuple exercises <exercises/lists/lists.rst>`_

------
quizes
------
* `Lists and Tuples Quiz <https://realpython.com/quizzes/python-lists-tuples/>`_
* `"while" Loops Quiz <https://realpython.com/quizzes/python-while-loop/>`_
