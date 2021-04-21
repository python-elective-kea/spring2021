Session 12 - Dataclasses 
========================

Materials
---------
* `Data Classes in Python 3.7+ (Guide) <https://realpython.com/python-data-classes/>`_
* `Code examples from teachings <https://github.com/python-elective-kea/spring2021-code-examples-from-teachings/tree/master/ses12>`_

Exercises
---------


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


