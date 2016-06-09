..  Copyright (C)  Brad Miller, David Ranum, Jeffrey Elkner, Peter Wentworth, Allen B. Downey, Chris
    Meyers, and Dario Mitchell.  Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Repeating an Operation a Fixed Number of Times
----------------------------------------------


As a special case, we might not care about the items that we are iterating through. We might just care about the number of times that we are iterating.

.. activecode:: ch08_3_1
	:nocanvas:

	for name in ["Joe", "Amy", "Brad", "Angelina", "Zuki", "Thandi", "Paris"]:
	    print "HELLO"


In the above for loop, the contents of the list were not the important part. The important part was that there were 7 items in the list so that HELLO was printed out 7 times. In fact, we did not even use name when we printed out HELLO! We can get the same result by simply using a list with any contents, however it makes more sense to people when we are looking at it if we used numbers. By running this code, you'll see that while the contents of the list that are being iterated over have changed, the end result, 7 HELLO's, has not changed.

.. activecode:: ch08_3_2
	:nocanvas:

	for n in [0, 1, 2, 3, 4, 5, 6]:
	    print "HELLO"

It is easy enough to write this list when the numbers are small, perhaps we only want to iterate over something 5 times or 9 times. However, what if we wanted to iterate over something 50 times or 100 times?

.. activecode:: ch08_3_3
	:nocanvas:

	for n in [0, 1, 2, 3, 4]: 
	    print "HELLO"
	print "This HELLO printed 5 times"

	for a in [0, 1, 2, 3, 4, 5, 6, 7, 8]:
	    print "HELLO"
	print "This HELLO printed 9 times"

	for item in [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, 64, 65, 66, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99]:
	    print "HELLO"
	print "This HELLO printed 100 times"

You can see how it might become a bit frustrating if, when we wanted to iterate over something 100 times, we had to type out a list that contained 100 items. Conveniently, we can use the ``range`` function to automatically generate a list of numbers. For example, range(5), produces a list of five numbers, starting with 0, [0, 1, 2, 3, 4].

.. activecode:: ch08_3_4
	:nocanvas:

	print range(5)
	print range(9)
	print range(100)

Now, when we want to iterate a fixed number of times, we are able to do so quickly and easily. Imagine now if we wanted to say hello 100 times, it would be much more simple.

.. activecode:: ch08_3_5
	:nocanvas:

	for item in range(100):
	    print "HELLO"

In some cases, it may be more helpful to start at a number other than 0. What if we wanted to create a list that went from 1 to 5, not 0 to 4? Thankfully, the range function provides an optional parameter that can let us do just that. By using 2 parameters, we can specify the beginning number that is used for the generated list. It is important to note though, that like taking slices of sequences, it is inclusive of the first number and exclusive of the second number.

.. activecode:: ch08_3_6
	:nocanvas:

	print range(5)
	print range(0, 5)

	print range(1, 6)

**Check your Understanding**

.. mchoicema:: test_question08_3_1
	:answer_a: range(3)
	:answer_b: [1, 2, 3]
	:answer_c: range(0, 3)
	:answer_d: [0, 1, 2]
	:answer_e: [3]
	:feedback_a: Yes, this creates [0, 1, 2]!
	:feedback_b: Not quite, this is a list of three elements, but are they the same elements as are in the equivalent lists?
	:feedback_c: Yes, this creates [0, 1, 2]!
	:feedback_d: Yes, this list matches those created using range.
	:feedback_e: This just is a list with one element, the integer 3.
	:correct: a,c,d

	Which of these answers are equivalent? (choose all that apply)

.. mchoicemf:: test_question08_3_2
	:answer_a: It tells a for loop how far to go.
	:answer_b: It prints something the specifed amount of times.
	:answer_c: It automatically generates a list of numbers.
	:feedback_a:  Not necessarily, you don't have to use range just with for loops.
	:feedback_b: While range can be used to specify a certain number of times that something is done, it has nothing to do with printing.
	:feedback_c: 
	:correct: c 

	What does ``range`` do?


