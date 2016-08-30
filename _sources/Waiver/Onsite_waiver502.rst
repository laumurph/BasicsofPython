..  Copyright (C) Lauren Murphy and Paul Resnick.  Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

:orphan:

.. qnum::
   :prefix: waiver502_
   :start: 1

.. highlight:: python
    :linenothreshold: 500

502 Waiver Exam Page
====================

The following is the assessment for the 502 Waiver. This should take about 30 minutes to complete. It tests your understanding of the basic mechanics of:

* Assignment statements
* Conditional execution
* Indexing into strings and lists
* For loops
* Dictionaries

502 Waiver Exam
---------------

**Instructions:** For questions that ask you to write code, write code in the provided active code windows and click the Run button. Feel keep editing the code until you get feedback that you have passed the tests. The last code you run for each problem will be graded. Instructions are comments in the code windows. *Do not* hit **Finish Exam** until you are finished.

.. activecode:: waiver502_1
  :nocodelens:
  :autograde: unittest

  # Create a variable called uni and assign it the value:
  # "University of Michigan"

  =====

  from unittest.gui import TestCaseGui

  class myTests(TestCaseGui):

     def testOne(self):
        self.assertEqual(uni, "University of Michigan", "Checking value of variable uni")

  myTests().main()



.. mchoice:: waiver502_9
  :autograde: first_answer
  :answer_a: String
  :answer_b: List
  :answer_c: Dictionary
  :feedback_a: Because you took a slice, the resulting type will be a list.
  :feedback_b: Because you took a slice, the resulting type will be a list.
  :feedback_c: Because you took a slice, the resulting type will be a list.
  :correct: b

  After the following Python code is executed, what will be the type of L[4:5] if L = ['p', 'y', 't', 'h', 'o', 'n']?


.. mchoice:: waiver502_11
  :autograde: first_answer
  :answer_a: 6
  :answer_b: 3
  :answer_c: False
  :answer_d: True
  :answer_e: None of the above, there will be an error.
  :feedback_a: First was compared against sec, not combined with sec + 1, it is still 3.
  :feedback_b: First still is assigned the value of 3, even after the comparison against sec + 1.
  :feedback_c: First is not reassigned the value of the comparison of first and sec + 1, which would have been True, not False, so first is still 3.
  :feedback_d: First is not reassigned the value of the comparison of first and sec + 1, so it cannot be True. First is still 3.
  :feedback_e: No error occurs, all of the lines are permissible in python.
  :correct: b

  What will print out at the end of this section of code?

  .. sourcecode:: python

     first = 3
     sec = 2
     first == sec + 1
     print first

.. mchoice:: waiver502_14
  :autograde: first_answer
  :answer_a: True
  :answer_b: False
  :answer_c: 'b'
  :answer_d: 4
  :answer_e: Error occurs
  :feedback_a: Using the in opperator on dictionaries checks the keys, so since 4 is not a key, it will return False.
  :feedback_b: Using the in opperator on dictionaries checks the keys, so since 4 is not a key, it will return False.
  :feedback_c: When using the in opperator on dictionaries, it checks the keys and would not find the 4. Additionally, the in opperator returns a boolean value, not the key associated with a value.
  :feedback_d: When using the in opperator on dictionaries, it checks the keys and would not find the 4. Additionally, the in opperator returns a boolean value, not the value it checks for.
  :feedback_e: The in opperator is permissible in python, and returns a boolean value.
  :correct: b

  What will print when this code is run?

  .. sourcecode:: python

     d = {}
     d['a'] = 5
     d['b'] = 4
     d[3] = 'b'
     print 4 in d


.. activecode:: waiver502_22
  :nocodelens:
  :autograde: unittest

  # Without changing the existing code, write a new line of code
  # to change the number of students
  # who are in Information so that there are 490 students.

  enrollment = {"Architecture": 638, "InterArts": 15, "Law": 885, "Pharmacy": 420, "Information": 459, "LSA": 18290, "Engineering": 8723, "Social Work": "472"}

  =====

  from unittest.gui import TestCaseGui

  class myTests(TestCaseGui):

     def testOne(self):
        self.assertEqual(enrollment["Information"], 490)

  myTests().main()


.. mchoice:: waiver502_24
  :autograde: first_answer
  :answer_a: You have been late more than tardy.
  :answer_b: You are just as late as you are tardy.
  :answer_c: You are more tardy than late.
  :answer_d: You might be more tardy.
  :answer_e: You're less tardy.
  :feedback_a: While that did happen at first, the program continues and this is overwritten.
  :feedback_b: Not quite!
  :feedback_c: Not quite!
  :feedback_d: Not quite!
  :feedback_e: Correct!
  :correct: e

  What will be printed?

  .. sourcecode:: python

     tardy = 4
     late = 8
     res = ""

     if late > tardy:
        res = "You have been late more than tardy."
     elif late == tardy:
        res = "You are just as late as you are tardy."
     else:
        res = "You are more tardy than late."

     if tardy >= late:
        res = "You might be more tardy."
     else:
        res = "You're less tardy."

.. activecode:: waiver502_23
  :nocodelens:
  :autograde: unittest

  # Write code to iterate through the numbers in lst,
  # printing out double each value.
  # Your output should be:
  # 2
  # 4
  # 6
  # 8
  # 10

  lst = [1, 2, 3, 4, 5]

.. activecode:: waiver502_8
  :nocodelens:
  :autograde: unittest


  # Write a statement to assign the second to last word in this
  # string to the variable called scri. Hint: use the split method.

  sent = "The Michigan Difference is a wonderful motto."

  =====

  from unittest.gui import TestCaseGui

  class myTests(TestCaseGui):

     def testOne(self):
        self.assertEqual(scri, sent.split()[-2])

  myTests().main()

