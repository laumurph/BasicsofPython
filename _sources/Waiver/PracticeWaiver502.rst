:orphan:
.. qnum::
   :prefix: pwaiver502_
   :start: 1

..  Copyright (C) Paul Resnick.  Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".


.. highlight:: python
    :linenothreshold: 500


.. 22 problems in the practice assessment

Practice Assessment for 502 Waiver
::::::::::::::::::::::::::::::::::

The following is the practice assessment for the 502 Waiver. This should take about 30 minutes to complete. Content for the assessment is based on the Basics of Python chapter.

**Instructions** For questions that require you to write code, write the code you want to save in the provided boxes. This is not a timed assessment, but feel free to keep track of how long it takes you to complete this page as an idicator of how well you will be prepared should you go straight into 506.

.. mchoicemf:: pwaiver_mc_1
   :answer_a: "Hello, world!"
   :answer_b: Hello, world!
   :answer_c: An error occurs, you have not initialized the type of the variable.
   :feedback_a: When printing a string, the quotes are not included.
   :feedback_b: When printing a string, the quotes are not included.
   :feedback_c: Python does not require that you initialize your variable's type.
   :correct: b

   What is the output when this code is run?

   .. sourcecode:: python

      first_prog = "Hello, world!"
      print first_prog

.. mchoicema:: pwaiver_mc_2
   :answer_a: var[2]
   :answer_b: var[2:3]
   :answer_c: var["g"]
   :answer_d: var[-8]
   :feedback_a: This refers to the substring "g".
   :feedback_b: Instead of being a string type, this one is a list because it used slicing.
   :feedback_c: An Error occurs because when indexing, you must use the numerical position.
   :feedback_d: This refers to the substring "g".
   :correct: a,d

   Which of these are equivalent? (Choose all that apply)

   .. sourcecode:: python

      var = "Big House!"

.. mchoicemf:: pwaiver_mc_3
   :answer_a: 23
   :answer_b: 26
   :answer_c: 22
   :answer_d: 25
   :answer_d: An Error occurs, incorrect use of len function.
   :feedback_a: Spaces are counted as characters and are accounted for when using the len function.
   :feedback_b: There are 26 characters.
   :feedback_c: Spaces and puncuation are counted as characters and are accounted for when using the len function.
   :feedback_d: The len function can take a variable as input, this does not cause an error.
   :feedback_e: The len function returns the number of characters that are found in what is inputted. Unlike indexing, it will start with 1, not 0. 
   :correct: b

   Which is these is the correct number produced by the following code?

   .. sourcecode:: python

      sent = "Welcome to the University."
      print len(sent)

.. mchoicema:: pwaiver_mc_4
   :answer_a: When doing calculations to denote what should be done first.
   :answer_b: Creating lists.
   :answer_c: Calling a function.
   :answer_d: Creating dictionaries.
   :feedback_a: You are able to use them when doing calculations.
   :feedback_b: Lists use [] as brackets, not ().
   :feedback_c: We use them in order to call or invoke a function.
   :feedback_d: Dictionaries use {} as brackets, not ().
   :correct: a,c

   Where can you use ``()`` in programming so far? (choose all that apply)

Save the value of the (human) 5th position in the list into a variable called ``abc``.

.. activecode:: pwaiver_a_1 
   :nocodelens:

   zxy = [1, 2, 30, "sims", ["Hello", 9.4, "World", "python"], 502, 506]

   =====

   from unittest.gui import TestCaseGui

   class myTests(TestCaseGui):

      def testOne(self):
         self.assertEqual(abc, ["Hello", 9.4, "World", "python"], "Your assignment does not align with the correct position in the list.")

   myTests().main()

.. parsonsprob:: pwaiver_pp_1
   
   Arrange the following code snipits into the correct order so that if new_class is larger than or equal to 506 then it will print "You might be going into 506." If new_class is smaller than 502, print "Have you applied to the school?" Otherwise, print "This is the waiver."

   -----
   new_class = 502
   =====
   if new_class >= 506:
   =====
       print "You might be going to 506."
   =====
   elif new_class < 502:
   =====
       print "Have you applied to the school?"
   =====
   else:
   =====
       print "This is the waiver."

.. mchoicemf:: pwaiver_mc_5
   :answer_a: False
   :answer_b: True
   :feedback_a: You can have an if statement that does not have an elif and/or else.
   :feedback_b: You can have an if statement that does not have an elif and/or else.
   :correct: b

   True or false, you may have an if statement without an elif and/or else?

.. mchoicema:: pwaiver_mc_6
   :answer_a: num = num + 1
   :answer_b: num ++
   :answer_c: num ++ 1
   :answer_d: num += 1
   :feedback_a: correct, num would be reassigned the value of num plus 1.
   :feedback_b: This is not permissible in python, an Error would occur.
   :feedback_c: This is not permissible in python, an Error would occur.
   :feedback_d: correct, num would be reassigned the value of num plus 1.
   :correct: a,d

   Which snipit of code would increment the value of ``num`` by one? (choose all that apply) 

Using the variable ``wrds``, how might you grab the last seven characters of a string? Save the last 7 characters of ``wrds`` in a variable called ``plc`` so that when plc is printed out, the output would be: States.

.. activecode:: pwaiver_a_2
   :nocodelens:

   wrds = "Summer is a warm time of year in the United States."

   =====

   from unittest.gui import TestCaseGui

   class myTests(TestCaseGui):

      def testOne(self):
         self.assertEqual(plc, wrds[-7:], "plc does not contain the correct characters.")

   myTests().main()

.. parsonsprob:: pwaiver_pp_2

   Organize the code snipits so that if the string "venmo" is an element of the list, then it prints out True, otherwise, it print False.

   -----
   lst = ["I use venmo", 
         "I owe my friend 10 dollars for pizza", 10, 
         {"pizza": 10, "burger": -7.59, "park": -2.25}]
   =====
   if "venmo" in lst:
   =====
      print True
   =====
   else:
   =====
      print False

.. mchoicemf:: pwaiver_mc_7
   :answer_a: 1
   :answer_b: 4
   :answer_c: 5
   :answer_d: 8
   :feedback_a: The last element is a list, so the len function returns the length of that list.
   :feedback_b: We are using len on a single element of the list lst_test, so it will only be the len of that element, not the whole list.
   :feedback_c: We are using len on the last element of the list which is four!
   :feedback_d: Since we are using negative indicies, we will not use "Good-bye", we will use the last element, which is the list [10, 9, [], "good night"]
   :correct: b

   What is returned at the end of this program?

   
   .. sourcecode:: python

      lst_test = ["Hello", "Good-bye", "Good day", 35.9, [10, 9, [], "good night"]]
      print len(lst_test[-1])

Using the two variables listed, combine them together and save that in a variable called ``combo`` so that if combo was printed, the resulting string would be "The arb was a great place to vist this week!"

.. activecode:: pwaiver_a_3
   :nocodelens:

   place = "The arb was a great place "
   feel = "to visit this week!"

   =====

   from unittest.gui import TestCaseGui

   class myTests(TestCaseGui):

      def testOne(self):
         self.assertEqual(combo, place + feel, "You have not correctly concatinated the two variables.")

   myTests().main()

.. mchoicema:: pwaiver_mc_8
   :answer_a: range(0, hbe)
   :answer_b: range(hbe)
   :answer_c: range(16)
   :answer_d: range() = hbe
   :feedback_a: This will produce a list that contains elements between 0 and 15.
   :feedback_b: This will produce a list that contains elements between 0 and 15.
   :feedback_c: While this would produce the correct length of a list of numbers, this is considered hardcoding. Imagine we didn't know what the string was, how would you do it then?
   :feedback_d: This would cause an error because it attempts to assign, to a function call, the value of a string. That is not permitted in Python.
   :correct: a, b

   Which snipit of code would produce a list of numbers with as many elements as this string without hardcoding? (Choose all that apply)

   .. sourcecode:: python

      hbe = "Python is great."

.. parsonsprob:: pwaiver_pp_3

   Organize the code snipits so that "Go blue!" and "Go maize!" are printed out alternately, 4 times.

   -----
   wow = "Go blue!"
   =====
   for i in range(4):
   =====
      print wow
   =====
      print "Go maize!"

.. mchoicema:: pwaiver_mc_9
   :answer_a: True
   :answer_b: true
   :answer_c: False
   :answer_d: false
   :feedback_a: True with a capital T is the boolean value.
   :feedback_b: True with a lowercase t is not a boolean, it's a variable in this case.
   :feedback_c: False with a capital F is the boolean value.
   :feedback_d: False with a lowercase f is not a boolean, it's a variable in this case.
   :correct: a,c

   Which are the boolean values? (Choose all that apply)

Save the length of each element in the list in a new list called ``len_vals``.

.. activecode:: pwaiver_a_4
   :nocodelens:

   vals = ["Python", "summer time", "Hello World!", "onomonopia", "Floccinaucinihilipilification", "supercalifragilisticexpialidocious", "wheel", "copyright", "fall", "School of Information"]

   =====

   from unittest.gui import TestCaseGui

   class myTests(TestCaseGui):

      def testOne(self):
         self.assertEqual(len_vals, [6, 11, 12, 10, 29, 34, 5, 9, 4, 21], "You have not correctly created a list with the lengths of the elements in the vals variable.")

   myTests().main()

.. mchoicemf:: pwaiver_mc_10
   :answer_a: dict = value[key]
   :answer_b: dict[key] = value
   :answer_c: dict = key[value]
   :answer_d: dict[value] = key
   :feedback_a: In order to create a new key value pair, the key must be next to the dictionary on the left side in order to reference the value and the value must be on the right side of the assignment statement.
   :feedback_b: The key is used on the left side of the assignment statement and the value is on the right side of the assignment statement.
   :feedback_c: In order to create a new key value pair, the key must be next to the dictionary on the left side in order to reference the value and the value must be on the right side of the assignment statement.
   :feedback_d: In order to create a new key value pair, the key must be on the right side of the assignment statement because it is used to reference the value, which is on the left side of the assignment statement.
   :correct: b

   How can you add a new key value pair to a dictionary?

.. mchoicemf:: pwaiver_mc_11
   :answer_a: indecies
   :answer_b: keys
   :answer_c: function calls
   :feedback_a: Indecies are used for things like strings and lists, but not for dictionaries.
   :feedback_b: Dictionaries use keys to access their information.
   :feedback_c: Function calls are not a way to access a dicitonary, they are used to use a function.
   :correct: b

   How are dictionaries accessed?

Create a dictionary called ``extra`` that has the key-value pairs: "Black" and "White", 14.9 and 0, "milkshake" and 390, and 29 and an empty list.

.. activecode:: pwaiver_a_5
   :nocodelens:

   =====

   from unittest.gui import TestCaseGui

   class myTests(TestCaseGui):

      def testOne(self):
         self.assertEqual(sorted(extra), sorted({"Black": "White", 14.9: 0, "milkshake": 390, 29: []}), "The dictionary was not set up correctly.")
         self.assertEqual(sorted(extra.values()), sorted(["White", 0, 390, []]), "The values of your dictionary do not match what is expected.")


   myTests().main()


.. mchoicemf:: pwaiver_mc_12
   :answer_a: the last value
   :answer_b: the last key
   :answer_c: the values
   :answer_d: the keys
   :answer_e: the word item
   :feedback_a: This will print out all of the keys, not one value. If we wanted to print out the 'last' value, we would have had to use the key that was associated with it to access the value and it would not have occured in the for loop.
   :feedback_b: This will print out all of the keys. If we wanted to print out the 'last' one just once, we wouldn't have put the print item statement in the for loop.
   :feedback_c: Item refers to the keys in the dictionary. If we wanted to print the values, then we would have needed to use the keys to access the values.
   :feedback_d: Item refers to the keys in the dictionary.
   :feedback_e: Item is not a string this case, it is a variable that refers to the keys in the dictionary.
   :correct: d

   What part of a dictionary is printed out at the end of the following statements?

   .. sourcecode:: python

      mydict = {True: False, "lol": "laugh out loud",
               "bark": 2, 40; 20, 
               "wonderful: ["incredible", "fabulous", "awful nice"]}
      for item in mydict:
         print item

Create a list of numbers starting at 15 and goes to 145 and assign that to a variable called ``big_lst``.

.. activecode:: pwaiver_a_6
   :nocodelens:

   =====

   from unittest.gui import TestCaseGui

   class myTests(TestCaseGui):

      def testOne(self):
         self.assertEqual(big_lst, [15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, 64, 65, 66, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99, 100, 101, 102, 103, 104, 105, 106, 107, 108, 109, 110, 111, 112, 113, 114, 115, 116, 117, 118, 119, 120, 121, 122, 123, 124, 125, 126, 127, 128, 129, 130, 131, 132, 133, 134, 135, 136, 137, 138, 139, 140, 141, 142, 143, 144, 145], "Your list does not cover the correct range")

   myTests().main()

.. mchoicemf:: pwaiver_mc_13
   :answer_a: True
   :answer_b: False
   :answer_c: 10
   :answer_d: 4
   :answer_e: An Error occurs.
   :feedback_a: a is reassigned the value produced by the statement b == 10, which checks equivalency and is thus True.
   :feedback_b: a is reassigned the value produced by the statement b == 10, which checks equivalency and is thus True because b has been reassigned the value of a (which was 10).
   :feedback_c: a is reassigned the value produced by the statement b == 10, which checks equivalency and is thus True because b has been reassigned the value of a (which had been 10 earlier).
   :feedback_d: a is reassigned the value produced by the statement b == 10, which checks equivalency and is thus True because b has been reassigned the value of a (which had been 10 earlier).
   :feedback_e:
   :correct: a

   What prints out at the end of this code?

   .. sourcecode:: python

      b = 4
      a = 10
      b = a
      a = b == 10
      print a




