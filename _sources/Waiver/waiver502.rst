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


502 Waiver Exam Page
====================


The following is the assessment for the 502 Waiver. This should take about 30 minutes to complete. Content based on the first few chapters will include:

* Assignment Statements
* Conditional Statements
* Indexing
* For Loops
* Dictionaries


502 Waiver Exam
---------------

.. .. datafile  about_programming.txt
..    :hide:

..    Computer programming (often shortened to programming) is a process that leads from an
..    original formulation of a computing problem to executable programs. It involves
..    activities such as analysis, understanding, and generically solving such problems
..    resulting in an algorithm, verification of requirements of the algorithm including its
..    correctness and its resource consumption, implementation (or coding) of the algorithm in
..    a target programming language, testing, debugging, and maintaining the source code,
..    implementation of the build system and management of derived artefacts such as machine
..    code of computer programs. The algorithm is often only represented in human-parseable
..    form and reasoned about using logic. Source code is written in one or more programming
..    languages (such as C++, C#, Java, Python, Smalltalk, JavaScript, etc.). The purpose of
..    programming is to find a sequence of instructions that will automate performing a
..    specific task or solve a given problem. The process of programming thus often requires
..    expertise in many different subjects, including knowledge of the application domain,
..    specialized algorithms and formal logic.
..    Within software engineering, programming (the implementation) is regarded as one phase in a software development process. There is an on-going debate on the extent to which
..    the writing of programs is an art form, a craft, or an engineering discipline. In
..    general, good programming is considered to be the measured application of all three,
..    with the goal of producing an efficient and evolvable software solution (the criteria
..    for "efficient" and "evolvable" vary considerably). The discipline differs from many
..    other technical professions in that programmers, in general, do not need to be licensed
..    or pass any standardized (or governmentally regulated) certification tests in order to
..    call themselves "programmers" or even "software engineers." Because the discipline
..    covers many areas, which may or may not include critical applications, it is debatable
..    whether licensing is required for the profession as a whole. In most cases, the
..    discipline is self-governed by the entities which require the programming, and sometimes
..    very strict environments are defined (e.g. United States Air Force use of AdaCore and
..    security clearance). However, representing oneself as a "professional software engineer"
..    without a license from an accredited institution is illegal in many parts of the world.

**Instructions:** For questions that ask you to write code, write the code you want to save in the provided boxes. The last code you have saved for each one by the deadline is what will be graded. Instructions are comments in the code window. *Do not* hit **Finish Exam** until you are finished. 



.. timed:: timed1
   :timelimit: 30


   .. activecode:: waiver502_1
      :nocodelens:

      # Create a variable called uni and assign it the value of 
      # this phrase: University of Michigan
      
      

      =====
      import test
      try: 
         test.testEqual(uni, "University of Michigan")
      except:
         print "Either uni has not been named correctly or has not been assigned the value of the string, 'University of Michigan'"


   .. parsonsprob:: waiver502_2
      
      Arrange the following code snipits in the correct order to loop through the list and print out only those that are integers, otherwise print None.

      -----
      full_list = ["Hello", 5, "world", -7.3,
                  ["umich", "edu"], -1817, 0.000,
                   "runestone"]
      =====
      for item in full_list:
      =====
         if type(item) == int:
      =====
            print item
      =====
         else:
      =====
            print "None"


   .. mchoicemf:: waiver502_3
      :answer_a: Integer
      :answer_b: Float
      :answer_c: String
      :answer_d: List
      :feedback_a: a working
      :feedback_b: b working
      :feedback_c: c working
      :feedback_d: d working
      :correct: c

      What is the type of "6.2" ?


   .. mchoicemf:: waiver502_4
      :answer_a: Integer
      :answer_b: Float
      :answer_c: String
      :answer_d: List
      :answer_e: Dictionary
      :feedback_a: a working
      :feedback_b: b working
      :feedback_c: c working
      :feedback_d: d working
      :feedback_e: e working
      :correct: d

      What is value of the (human) fifth position in this list: ["School", "Ann Arbor", "93.0", 38, [6], "Information", {3: "three", "Six": 6, 109: 109.0}]?


   .. activecode:: waiver502_5
      :nocodelens:

      # Write code so that var is printed out 8 times, each time
      # on a new line, without writing 8 print statements (hardcoding).

      var = "9"
   

   .. activecode:: waiver502_6
      :nocodelens:

      # Print out the type of each item in the list on a separate line.

       lst = [["Dog", "cat", 8], "pet", {"Lassie": "dog", "Porky": "pig"}, 10, 9, 8.99]


   .. activecode:: waiver502_7
      :nocodelens:
      :include: addi_functions



      #len and range of 5 as a replacement for this, length of list

      # We are providing a function called square() which takes as
      # input, one integer and returns the square of that integer 
      # value. Write code to assign the variable abc the value of 285
      # squared divided by 3. Use the square function in your answer.

      def square(num):
        return num**2

      abc = ""

      =====
      import test

      try: 
         test.testEqual(uni, "University of Michigan")
      except:
         print "Either uni has not been named correctly or has not been assigned the value of the string, 'University of Michigan'"
 

   .. activecode:: waiver502_8
      :nocodelens:

      # Write a statement to print the second to last word in any
      # string, assuming it has at least two words. For example,
      # when sent is defined, you would be printing out the word wonderful. 

      sent = "The Michigan Difference is a wonderful catchphrase."


   .. mchoicemf:: waiver502_9
      :answer_a: Integer
      :answer_b: Float
      :answer_c: String
      :answer_d: List
      :answer_e: Dictionary
      :feedback_a: A working
      :feedback_b: B working
      :feedback_c: C working
      :feedback_d: D working
      :feedback_e: E working
      :correct: d

      After the following Python code is executed, what will the the type of L[4:5] if L = ['p', 'y', 't', 'h', 'o', 'n']?


   .. activecode:: waiver502_10
      :nocodelens:

      # Write code so that the number of times the letter **a**
      # is written in the string provided is saved as the value
      # of a variable called num_of_a.

      sent_long = "Programming is a useful skill for people to know in this day and age, where computers are an important and vital tool in societies."


   .. mchoicemf:: waiver502_11
      :answer_a: 5
      :answer_b: 3
      :answer_c: False
      :answer_d: True
      :answer_e: None of the above, there will be an error.
      :feedback_a: A working
      :feedback_b: B working
      :feedback_c: C working
      :feedback_d: D working
      :feedback_e: E working
      :correct: d
      
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

      # Using the dictionary provided, print out each key 
      # value pair on a separate line, but only if the value
      # contains the letter **m**.

      word_dict = {"yellow": "maize", "blue": "same thing", "NQ": "North Quad", "UMSI": "University of Michigan School of Information", "A2": "Ann Arbor", "Big House": "The Football Stadium", "Language": "Python", "Fishbowl": "Computing Site"}

      # It should look something like this:

      # yellow maize
      # blue same thing
      # UMSI University of Michigan School of Information
      # Big House The Football Stadium
      # Fishbowl Computing Site

      # the order may be different, but there should be 
      # no more and no fewer pairs


   .. mchoicemf:: waiver502_14
      :answer_a: True
      :answer_b: False
      :answer_c: 'b'
      :answer_d: 4
      :answer_e: Error occurs
      :feedback_a: A working
      :feedback_b: B working
      :feedback_c: C working
      :feedback_d: D working
      :feedback_e: E working
      :correct: b

      What would occur when this code is printed?

      .. sourcecode:: python

         d = {}
         d['a'] = 5
         d['b'] = 4
         d[3] = 'b'
         print 4 in python


   .. activecode:: waiver502_15
      :nocodelens:

      # Accumulate the values so that the total number is displayed in output like so: This is my 29th favorite day of the month.
      # Save this in a variable called **fav_day**.

      num_dict = {"University of Michigan": 19, "month": 4, "student": 3.5, "season": 2, "question": .5}

   .. mchoicema:: waiver502_16
      :answer_a: There is a list and a dictionary inside of the dictionary
      :answer_b: There is no assignment statement
      :answer_c: Some of the values and keys are missing quotes
      :answer_d: There's a comma missing
      :answer_e: a number is a key, which is not allowed
      :feedback_a: Not quite right, you are allowed to have dictionaries and lists inside of other lists and dictionaries.
      :feedback_b: 
      :feedback_c: 
      :feedback_d: 
      :feedback_e: Not quite right, numbers are allowed to be keys and values.
      :correct: b,c,d

      What is wrong with this dictionary?

      .. sourcecode:: python

         {"diction": ary, "gaming consoles": ["ps4", "gamecube", "xbox360", "nintendo64", "Atari"], "phones": 3 "broken": 10, donut: {"Glazed": 10, 2: "blueberry", "Chocolate": "Many"}}


   .. activecode:: waiver502_17
      :nocodelens:
      :include: addi_functions

      # We have provided a function called **random_digit()** which takes no inputs and produces a number between 0 and 9
      # Using this function, print whether or not the resulting number is above 6, below 3, or inbetween. 
      # If it is above 6, print "The random number generated is above 6", if it is below 3, print "The random number 
      # generated is below 3", and if it is between, print "The random number generated is between 3 and 6".

   .. activecode:: waiver502_18
      :nocodelens:
      :include: addi_functions

      # Iterate through the list of integers so that, using the **square()** function, if the resulting value is 
      # divisable by 4 with zero remaining, then the original number is saved into a new list called **div_four**, 
      # otherwise save it to a new list called **not_div_four**.


      lst_nums = [9, 392, 4, 10, 244, 206, 506, 1983, 1817, 16]


   .. mchoicemf:: waiver502_19
      :answer_a: Yes, you can index into a dictionary by using their positions.
      :answer_b: Yes, you can index into a dictionary because they are like lists, just with {} brackets instead of [] ones. 
      :answer_c: No, you cannot index into a dictionary because they do not have positions.
      :answer_d: No, you cannot index into a dictionary because the {} brakets are different than then [] ones.
      :feedback_a: Dictionaries don't have positions that you can use to index.
      :feedback_b: Dictionaries aren't quite like lists, they are unordered whereas lists are ordered.
      :feedback_c: Correct!
      :feedback_d: They are different kinds of brakets, but that's not the reason why you can't index into a dictionary.
      :correct: c

      Can you index into a dictionary?

   .. mchoicemf:: waiver502_20
      :answer_a: "Zero"
      :answer_b: Zero
      :answer_c: Error, you cannot index into a dictionary
      :feedback_a: Not quite, the quotes will not be printed out.
      :feedback_b: Correct!
      :feedback_c: No, this is not indexing into a dictionary, this refers to the value that is associated with the key.
      :correct: b

      What is printed by the following statement?

      .. sourcecode:: python
      
         new_dict = {"Pizza": 7, "Large": 2, "Medium": "Zero", "Extra-large": "5"}
         print new_dict["Medium"]


   .. activecode:: waiver502_21
      :nocodelens:

      # Write code so that the values of this list of students from different programs are increased by one.
      # This should work for any time it is asked (do not hardcode).

      students = [52, 45, 90, 18, 150, 390, 1029]


   .. activecode:: waiver502_22
      :nocodelens:

      # Write code to increase the number of students who are in Information so that there are 490 students.

      enrollment = {"architecture": 638, "InterArts": 15, "Law": 885, "Pharmacy": 420, "Information": 459, "LSA": 18290, "Engineering": 8723, "Social Work": "472"}


   .. activecode:: waiver502_23
      :nocodelens:

      # We have provided you with another function, this one is called **greeting()** and takes two optional inputs, the 
      # first is a string for the name and the second is an integer for the number of exclamation marks. 
      # Using variables called **default**, **dean**, and **excited**, save different uses of the function **greeting()**
      
      def greeting(name, num):
         return "Hello,", name + ", and welcome to umich" + num * "!"

      #### DO NOT change the function definition above this line (OK to add comments)

      # Save a basic function call to the variable called default, so that its value is the string "Hello, Student, and welcome to umich!"


      # Save a funtion call to the variable called dean, this time using the name of the dean of the school, Thomas Finholt, for the greetings.


      # Save a function call to the variable called excited, this time just changing the number of exclamation marks so that there are five of them.

   .. mchoicemf:: waiver502_24
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


.. .. activecode addi_functions
.. :nopre:
.. :hidecode:

.. def square(num):
..   return num**2

.. def random_digit():
..   import random
..   return random.choice([0,1,2,3,4,5,6,7,8,9])



.. .. mchoicemf waiver502_1
..    :answer_a: Syntax error
..    :answer_b: Analytic error
..    :answer_c: Runtime error
..    :answer_d: Semantic error
..    :feedback_a: A semantic error is an error in logic. In this case the program does not produce the correct output because the problem is not solved correctly. This would be considered a run-time error.
..    :feedback_b: A semantic error is an error in logic. In this case the program does not produce the correct output because the code can not be processed by the compiler or interpreter. This would be considered a syntax error.
..    :feedback_c: This will produce the wrong answer because the programmer implemented the solution incorrectly.  This is a semantic error.
..    :feedback_d: Cri
..    :correct: b

..    Which one of these is not an error?

.. .. mchoicema waiver502_3
.. :answer_a: Allows programers to see information from programs.
.. :answer_b: Learn what the type of a value is by visually seeing it.
.. :answer_c: Print out the program to a printer.
.. :answer_d: Displays a value on the screen.
.. :feedback_a: ahhhhh
.. :feedback_b: cri
.. :feedback_c: wll
.. :feedback_d: yay
.. :correct: a,d

.. What are the benefits of print statments? (choose all that are correct)

.. .. mchoicemf waiver502_8
..    :answer_a: None, an error occurs.
..    :answer_b: 7
..    :answer_c: 7.0
..    :answer_d: 1
..    :feedback_a: a working
..    :feedback_b: b working
..    :feedback_c: c working
..    :feedback_d: d working
..    :correct: b

..    What is the value of the expression 36 // 5?

.. Correct the following code so that the file is opened in order to read contents. Then, add to the code so that it prints out a list where each element of the list is a line of the text file.

.. .. activecode waiver502_13
..    :nocodelens:
      
..    file_name = about_programing.txt
..    f = open(f, 'r')


.. Write code so that if the word **computer** (and any variation such as computers, computing, etc.) is in the file about_programming.txt, it would print out the line that it was on.

.. .. activecode waiver502_15
..    :nocodelens:

.. for waiver502_17 if for some reason it extended...
.. =====
.. accum = 0
.. keys = dict.keys()
.. best_key = keys[0]
.. =====
.. for key in keys:
.. =====
..    if dict[key] > dict[best_key]:
.. =====
..       best_key = key


