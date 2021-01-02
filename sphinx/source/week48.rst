Week 48 - Problem-Solving with python
=====================================
Today we solve problems. The code you will use for doing this will primarely be through things you already know. 

We will start out by looking at what we did not manage to do last time ablout Decorators, mostly about what is in the contextlib library. And we will lokk at the SQlite exercise. 

Materials
---------
`Solution  <exercises/solution/48_problem_solving/solutions.rst>`_

.. raw:: html

        <iframe width="560" height="315" src="https://www.youtube.com/embed/XKu_SEDAykw" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


* `Google job interview <https://www.youtube.com/watch?v=XKu_SEDAykw>`_


* `Code examples from teachings <https://github.com/python-elective-kea/fall2020-code-examples-from-teachings/tree/master/w48>`_

Exercises
---------

* `Card Challange <notebooks/CardChallenge.ipynb>`_  (`Solution <exercises/solution/48_problem_solving/CardChallenge_solution.ipynb>`_)
* `Euler Project <notebooks/project_euler.ipynb>`_  (`Solution <exercises/solution/48_problem_solving/project_euler_solutions.ipynb>`_)

-------------
Hjemmearbejde
-------------
* I har fået et link til en undersøgelse fra forskning og uddannelsesministeriet. Mailen skulle indeholde ordet "uddannelseszome". Det vil være en kæmpe hjælp for KEA hvis i kunne udfylde den derhjemme. Den tager vist ca. en time at udfylde, så vi bruger ikke tid i undervisningen på det. Men hvis i kunne bruge tid på det derehjemme vil det være fedt!

I kan se en præsentationsvideo her:

.. raw:: html

        <iframe width="560" height="315" src="https://www.youtube.com/embed/y9RCt0CL9ps" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

..        -------------------------
        Ex 1: Tjek dit cpr-nummer
        -------------------------

        Dit CPR-nummer består af 10 cifre. De 6 første er din fødselsdato, din måned og de sidste to cifre i dit fødselsår: ddmmåå  fx 150949.

        De tre første efter stregen er et såkaldt løbenummer, fra 000-399 i forrige årtusinde.

        Det sidste ciffer er et kontrolciffer, fx 1.

        Du kan tjekke dit eget CPR-nummer efter denne fremgangsmåde, hvor hvert ciffer ganges med en konstant i denne rækkefølge 4,3,2,7,6,5,4,3,2

        Alle produkterne (cpr ciffer og konstant) summeres, så ved cpr nummeret 150949-0941 får man: 

        * 4 + 15 + 0 + 63 + 24 + 45 +0 + 27 + 8 = 186 


        | Summen divideres med 11: 
        | 186 : 11 = 16,0909...
        | Det hele tal 16 ganges med konstanten 11
        | 16 * 11 = 176. 
        | Der er altså 186 –176 = 10 til rest.
        | NB! Hvis divisionen med 11 går op, og der ikke er nogen rest, gives automatisk kontrol-ciffer 0!

        | Kontrolnummeret findes ved at trække denne rest (her 10) fra konstanten 1111 – 10 = 1 
        | Dette nummer - 150949-xxxx


