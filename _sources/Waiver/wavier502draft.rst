:orphan:
.. qnum::
   :prefix: waiver502_
   :start: 1

..  Copyright (C) Paul Resnick.  Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".
    Creation of Problems by Lauren Murphy with many based off of materials provided by Paul Resnick and Jackie Cohen

.. highlight:: python
    :linenothreshold: 500


502 First Draft Waiver Exam Page
================================


The following is the assessment for the 502 Waiver. This should take about 30 minutes to complete. Content is based on the first few chapters of Programs, Information, and People or the Basics of Python chapter in the programming placement site distributed earlier in the summer, and will include:

* Assignment Statements
* Conditional Statements
* Indexing
* For Loops
* Dictionaries


502 Waiver Exam
---------------

**Instructions:** For questions that ask you to write code, write the code you want to save in the provided active code windows. The last code you have saved for each problem by the deadline is what will be graded. Instructions are comments in the code window. *Do not* hit **Finish Exam** until you are finished. 



.. timed:: timed1
   :timelimit: 30


   .. activecode:: waiver502_1
      :nocodelens:

      # Create a variable called uni and assign it the value of 
      # this phrase: University of Michigan
      
      

      =====

      from unittest.gui import TestCaseGui

      class myTests(TestCaseGui):

         def testOne(self):
            self.assertEqual(uni, "University of Michigan", "Either uni has not been named correctly or has not been assigned the value of the string, 'University of Michigan'")

      myTests().main()


   .. parsonsprob:: waiver502_2
      
      Arrange the following code snipits in the correct order to loop through the list and print out only those that are integers and floats and to otherwise print None.

      -----
      full_list = ["Hello", 5, "world", -7.3,
                  ["umich", "edu"], -1817, 0.000,
                   "runestone"]
      =====
      for item in full_list:
      =====
         if type(item) == int:
            print item
      =====
         elif type(item) == float:
            print item
      =====
         else:
      =====
            print "None"

   .. mchoice:: waiver502_3
      :answer_a: Items that you need for creating the list produced by the range function.
      :answer_b: The elements of the list produced by the range function call.
      :answer_c: Nothing, that is an improper use of a for loop.
      :feedback_a: The only input that the range function needs is between the parenthesis in the function call, item is not used for that.
      :feedback_b: Elem represents each element in the list that is created by the range function call.
      :feedback_c: The range function can be used as the object that is iterated over in a for loop.
      :correct: b

      In the following for loop, what does ``item`` represent?

      .. sourcecode:: python

         for item in range(3,15):


   .. mchoice:: waiver502_4
      :answer_a: Integer
      :answer_b: Float
      :answer_c: String
      :answer_d: List
      :answer_e: Dictionary
      :feedback_a: The human fifth position in the list refers to [6], which is a list. The contents of the list are a subsection and their type is not accounted for when refering to the entire list object.
      :feedback_b: The human fifth position in the list refers to [6], which is a list.
      :feedback_c: The human fifth position in the list refers to [6], which is a list.
      :feedback_d: The human fifth position in the list refers to [6], which is a list.
      :feedback_e: The human fifth position in the list refers to [6], which is a list, as denoted by the square [] brackets.
      :correct: d

      What is type of the value of the (human) fifth position in this list: ["School", "Ann Arbor", "93.0", 38, [6], "Information", {3: "three", "Six": 6, 109: 109.0}]?


   .. parsonsprob:: waiver502_5

      Arrange the following code snipits so that var is printed out 8 times, each time on a new line.

      -----
      var = "9"
      =====
      for pos in range(8):
      =====
         print var


   .. activecode:: waiver502_6
      :nocodelens:

      # If the type of the last variable in lst is a float or an integer, then assign the value of the_type to be True, otherwise assign it to be False. the_type is currently assigned the value None.

      lst = [["Dog", "cat", 8], "pet", {"Lassie": "dog", "Porky": "pig"}, 10, 9, 8.99]
      the_type = None

      =====

      from unittest.gui import TestCaseGui

      class myTests(TestCaseGui):

         def testOne(self):
            self.assertEqual(the_type, True, "The if/else conditional statement has not been set up correctly or the value of the_type is not a Boolean.")

      myTests().main()


   .. activecode:: waiver502_7
      :nocodelens:

      # Write code to assign the variable abc the value that is produced
      # when the length of a string is the input of the range function. 
      # In this case, when the length of the string "Hello" is used,
      # a list is produced and is saved as the value of the variable abc.

      wrd = "Hello"


      =====

      from unittest.gui import TestCaseGui

      class myTests(TestCaseGui):

         def testOne(self):
            self.assertEqual(abc, [0, 1, 2, 3, 4], "abc has not been assigned the correct value. There may be impropper use of the len or range functions.")

      myTests().main()
 

   .. activecode:: waiver502_8
      :nocodelens:

      # Write a statement to assign the second to last word in this
      # string to the variable called scri.

      sent = "The Michigan Difference is a wonderful motto."

      =====

      from unittest.gui import TestCaseGui

      class myTests(TestCaseGui):

         def testOne(self):
            self.assertEqual(scri, "wonderful", "scri has not been correctly assigned the value of 'wonderful', possibly due to incorrect indexing.")

      myTests().main()


   .. mchoice:: waiver502_9
      :answer_a: String
      :answer_b: List
      :answer_c: Dictionary
      :feedback_a: Due to the way that L was indexed in to, the resulting type will be a list.
      :feedback_b: Due to the way that L was indexed in to, the resulting type will be a list.
      :feedback_c: Unless the element that is indexed in to is a dictionary, the type of the value will not be a dictionary. In this case, even though the element is a string, the way that it was indexed will result in a list with the single element.
      :correct: b

      After the following Python code is executed, what will the the type of L[4:5] if L = ['p', 'y', 't', 'h', 'o', 'n']?


   .. activecode:: waiver502_10
      :nocodelens:

      # Write code so that if the letter q is in the string
      # then the program should assign the string "q is present"
      # to a variable called sent_ans, otherwise, it should assign
      # that variable the value of "q is not present".

      sent_long = "Programming is a useful skill for people to know in this day and age, where computers are an important and vital tool in societies."

      =====

      from unittest.gui import TestCaseGui

      class myTests(TestCaseGui):

         def testOne(self):
            self.assertEqual(sent_ans, "q is not present", "Testing whether sent_ans has been correctly set up and assigned the right value.")

      myTests().main()


   .. mchoice:: waiver502_11
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

   .. parsonsprob:: waiver502_12

      Arrange the following code snipits in the correct order so that the list of letters creates a dictionary where in the key is the letter and the value is the number of times it has occured in the list.

      -----
      let_list = ['a', 't', 
            'm', 'i','c', 'i',
            'b', 'e', 'y', 'p',
            't', 's', 'c', 'a', 
            'l', 'i', 'a', 'y',
            's', 's', 'u', 'e',
            'e', 'd',]
      dict = {}
      =====
      for let in let_list:
      =====
         if let in dict:
      =====
            dict[let] += 1
      =====
         else:
      =====
            dict[let] = 1


   .. activecode:: waiver502_13
      :nocodelens:

      # Using the dictionary provided, add an extra
      # key value pair, whose key is the string festival 
      # and whose value is the string summer fest.

      word_dict = {"yellow": "maize", "blue": "same thing", "NQ": "North Quad", "UMSI": "University of Michigan School of Information", "A2": "Ann Arbor", "Big House": "The Football Stadium", "Language": "Python", "Fishbowl": "Computing Site"}

      =====

      from unittest.gui import TestCaseGui

      class myTests(TestCaseGui):

         def testOne(self):
            self.assertEqual(sorted(word_dict), sorted({"yellow": "maize", "blue": "same thing", "NQ": "North Quad", "UMSI": "University of Michigan School of Information", "A2": "Ann Arbor", "Big House": "The Football Stadium", "Language": "Python", "Fishbowl": "Computing Site", "festival": "summer fest"}), "Checking whether word_dict has the right keys.")
            self.assertEqual(sorted(word_dict.values()), sorted("maize", "same thing", North Quad", "University of Michigan School of Information", "Ann Arbor", "The Football Stadium", "Python", "Computing Site", "summer fest"), "Checking whether word_dict has the right values.")


      myTests().main()


   .. mchoice:: waiver502_14
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

      What would occur when this code is printed?

      .. sourcecode:: python

         d = {}
         d['a'] = 5
         d['b'] = 4
         d[3] = 'b'
         print 4 in d


   .. parsonsprob:: waiver502_15

      Arrange the code snipits so that the values of the dictionary are added together
      so that the total number is displayed in a string that reads "This is my 29th
      favorite day of the month." and is printed out.

      -----
      num_dict = {"University of Michigan": 19, "month": 4, "student": 3.5, "season": 2, "question": .5}
      
      num = 0
      =====
      for key in num_dict:
      =====
         num = num + num_dict[key]
      =====
      print "This is my " + num + "th favorite day of the month."


   .. mchoice:: waiver502_16
      :multiple_answers:
      :answer_a: There is a list and a dictionary inside of the dictionary
      :answer_b: There is no assignment statement
      :answer_c: Some of the values and keys are missing quotes
      :answer_d: There's a comma missing
      :answer_e: a number is a key, which is not allowed
      :feedback_a: Not quite right, you are allowed to have dictionaries and lists inside of other lists and dictionaries.
      :feedback_b: Yes, there is no assignment statement, thus there is no way to use the dictionary later on.
      :feedback_c: Yes, some of the values and keys that are supposed to be strings are missing quotes around them, thus the dictionary will think that they are missing variables and cause an error.
      :feedback_d: Yes, there is a comma missing, which would cause an error when trying to run. Syntax is important to running programs.
      :feedback_e: Not quite right, numbers are allowed to be keys and values.
      :correct: b,c,d

      What is wrong with this dictionary?

      .. sourcecode:: python

         {"diction": ary, "gaming consoles": ["ps4", "gamecube", "xbox360", "nintendo64", "Atari"], "phones": 3 "broken": 10, donut: {"Glazed": 10, 2: "blueberry", "Chocolate": "Many"}}


   .. activecode:: waiver502_17
      :nocodelens:

      # assign to the variable desti, strings that describe
      # whether or not the length of "Pip install" is above 15,
      # below 8, or inbetween. If it is above 15, assign it 
      # "The lenth of the string is greater than 15",
      # if it is below 8, assign it "The lenth of the string is 
      # less than 8", and if it is between, assign it 
      # "The length of the string is between 15 and 8".

      =====

      from unittest.gui import TestCaseGui

      class myTests(TestCaseGui):

         def testOne(self):
            self.assertEqual(desti, "The length of the string is between 15 and 8", "desti may have been assigned the incorrect string.")

      myTests().main()

   .. parsonsprob:: waiver502_18

      Arrange the code snipits so that the list of integers is iterated through so that if the resulting value is divisable by 3 with zero remaining, then "div by 3: " and the number is printed, otherwise nothing happens.

      -----
      lst_nums = [9, 392, 4, 10, 244, 206, 506, 1983, 1817, 16]
      =====
      for nums in lst_nums:
      =====
         if num % 3 == 0:
      =====
            print "div by 3: ", num


   .. mchoice:: waiver502_19
      :answer_a: Yes, you can index into a dictionary by using their positions.
      :answer_b: Yes, you can index into a dictionary because they are like lists, just with {} brackets instead of [] ones. 
      :answer_c: No, you cannot index into a dictionary because they do not have positions.
      :answer_d: No, you cannot index into a dictionary because the {} brackets are different than then [] ones.
      :feedback_a: Dictionaries don't have positions that you can use to index.
      :feedback_b: Dictionaries aren't quite like lists, they are unordered whereas lists are ordered.
      :feedback_c: You cannot index into a dictionary because thery lack positions to use for numeric indices.
      :feedback_d: They are different kinds of brackets, but that's not the reason why you can't index into a dictionary.
      :correct: c

      Can you index into a dictionary?

   .. mchoice:: waiver502_20
      :answer_a: "Zero"
      :answer_b: Zero
      :answer_c: Error, you cannot index into a dictionary.
      :feedback_a: Not quite, the quotes will not be printed out.
      :feedback_b: The value of the key will be printed out without quotes.
      :feedback_c: No, this is not indexing into a dictionary, this is refering to the value that is associated with the key.
      :correct: b

      What is printed by the following statement?

      .. sourcecode:: python
      
         new_dict = {"Pizza": 7, "Large": 2, "Medium": "Zero", "Extra-large": "5"}
         print new_dict["Medium"]


   .. activecode:: waiver502_21
      :nocodelens:

      # Write code so that the length of the list 
      # is assigned to a variable called student_len.

      students = [52, 45, 90, 18, 150, 390, 1029]


      =====

      from unittest.gui import TestCaseGui

      class myTests(TestCaseGui):

         def testOne(self):
            self.assertEqual(student_len, len(students), "You incorrectly assigned the value of student_len to be the length of students.")

      myTests().main()ac


   .. activecode:: waiver502_22
      :nocodelens:

      # Write code to change the number of students 
      # who are in Information so that there are 490 students.

      enrollment = {"Architecture": 638, "InterArts": 15, "Law": 885, "Pharmacy": 420, "Information": 459, "LSA": 18290, "Engineering": 8723, "Social Work": "472"}


   .. mchoice:: pwaiver_mc_2
   :multiple_answers:
   :answer_a: var[4:5]
   :answer_b: var[4]
   :answer_c: var["l"]
   :answer_d: var[-3]
   :feedback_a: This refers to the substring "l", not "lu", because the slice goes up to but does include position 5.
   :feedback_b: This refers to the substring "l".
   :feedback_c: An Error occurs because when indexing, you must use the numerical position.
   :feedback_d: This refers to the substring "g".
   :correct: a,b,d

   Which of these are equivalent? (Choose all that apply)

   .. sourcecode:: python

      var = "Go Blue!"


   .. mchoice:: waiver502_24
      :answer_a: "You have been late more than tardy."
      :answer_b: "You're less tardy."
      :answer_c: "You are more tardy than late."
      :feedback_a: While that did happen at first, the program continues and this is overwritten.
      :feedback_b: Correct!
      :feedback_c: Not exactly, not only does late happen to be greater than tardy, but there is another if else conditional that the program goes through.
      :correct: b 

      What would be saved to the value of detention at the end of the code?

      .. sourcecode:: python
      
         tardy = 4
         late = 8
         detention = ""

         if late > tardy:
            detention = "You have been late more than tardy."
         elif late == tardy:
            dentention = "You are just as late as you are tardy."
         else:
            dentention = "You are more tardy than late."

         if tardy >= late:
            detention = "You might be more tardy."
         else:
            detention = "You're less tardy."

   .. mchoice:: waiver502_25
      :answer_a: range(23, 90)
      :answer_b: range(22, 90)
      :answer_c: range(23, 89)
      :answer_d: range(22, 89)
      :feedback_a: Range, when given two inputs, will be inclusive of the first and exclusive of the second, so this will work!
      :feedback_b:Range, when given two inputs, will be inclusive of the first and exclusive of the second.
      :feedback_c:Range, when given two inputs, will be inclusive of the first and exclusive of the second.
      :feedback_d:Range, when given two inputs, will be inclusive of the first and exclusive of the second.
      :correct: a

      How would you use the range function to create a list that spans from 23 up to and including 89?

