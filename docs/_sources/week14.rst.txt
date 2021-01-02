Week 14 - Comprehensions
========================

.. sidebar:: Learning goals
    :subtitle: After this week you will be able to:
        
        - Use comprehensions instead of loops and list assignments in you python code. 


This weeks topic is Comprehensions. Our main focus will be on List Comprehensions, but will also cover set, tuple and dict comprehensions. 
The learning goal for this you can read in the sidebar, and the way to achieve this goal is to read and understand the materials, and do the exercises. To check yourself wheter or not your reached this goal, you should have a look at the solutions for the exercises and check this agains your solution.


Materials
---------

* `Notebook on List Comprehensions <notebooks/Comprehensions.ipynb>`_
* `Notebook on other Comprehension types <notebooks/more_on_comp.ipynb>`_
* `Code from today <../week14/code_from_today/>`_

Exercises
---------

--------------------
Ex 1: Basic listcomp
--------------------
`Solutions <notebooks/Comprehensions.ipynb>`_


1. Create a list of capital letters from the english alphabet.
2. Do the same, but exclude the 4 with the Unicode code point of 70, 75, 80 and 85.
3. Create a list of capital letters, but exclude every second between F & O
4. Create something that prints 

.. code:: python
   
   ['un-even and small', 2, 'un-even and small', 4, 
   'un-even and large', 6, 'un-even and large', 8, 
   'un-even and large']


--------------------
Ex 2: Basic Dictcomp
--------------------

`Solution <notebooks/more_on_comp.ipynb#Dictcomp-Challange>`_

1. Create a dictionary containing a deck of cards. The keys should be the elements from the colors set and the values should be the elements from the numbers list as a set.

.. code:: python

   colors = {'♠', '♡', '♢', '♣'}
   numbers = [2, 3, 4, 5, 6, 7, 8, 9, 10, 'J', 'Q', 'K', 'A']

   # The result should be like this:
   {'♢': {10, 2, 3, 4, 5, 6, 7, 8, 9, 'A', 'J', 'K', 'Q'},
    '♡': {10, 2, 3, 4, 5, 6, 7, 8, 9, 'A', 'J', 'K', 'Q'},
    '♣': {10, 2, 3, 4, 5, 6, 7, 8, 9, 'A', 'J', 'K', 'Q'},
    '♠': {10, 2, 3, 4, 5, 6, 7, 8, 9, 'A', 'J', 'K', 'Q'}}

-------------------
Ex 3: Deck of Cards
-------------------


1. Create a listcomp that produces a list of tuples containing all card in a deck. 

.. code:: python

   [('A','♠'), ('K','♣'), ... ] etc.

Solution:

.. code:: python
   
   numbers = list(range(2, 11)) + ['J', 'Q', 'K', 'A']
   [(i,chr(j)) for i in numbers for j in range(9824, 9828)]

-----------------------------------
Ex 4: List Comprehension chalenges.
-----------------------------------

`Solution <../week14/exercises/solution/list_comprehensions_challenge.py>`_

All the below exercieses, unless something else is stated, should be solved using: 

1. a normal for loop 
2. a list comprehension 

You should also run the 'timer' and 'memory usage' decorators on your new functions. (these where the exercises last week)

Try to see if you in anyway can optimize you code. (It is a good idea to test your solutions with large numbers and see how they react)

.. code:: python
   :linenos:


        # 1. Find all of the numbers from 1-1000 that are divisible by 7
        @timer
        @profile
        def divisible_by_7_loop():
                pass
        
                
        @timer
        @profile
        def divisible_by_7_comp():
                pass



        # 2. Find all of the numbers from 1-1000 that have a 3 in them

        # 3. Count the number of spaces in a string

        # 4. Remove all of the vowels in a string

        # 5. In a string made up of randomly generated words, generate a list of all words that have less than 4 letters

        # 6. Use a dictionary comprehension to count the length of each word in a sentence.

        # 7. Use a nested list comprehension to find all of the numbers from 1-1000 that are divisible by any single digit besides 1 (2-9)

        # 8. For all the numbers 1-1000, use a nested list comprehension to find the highest single digit any of the numbers is divisible by

        # 9. Multiples of 3 and 5: If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23. Find the sum of all the multiples of 3 or 5 below 1000.





