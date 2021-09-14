Mixed-up code Questions
-----------------------

.. parsonsprob:: ch5ex1muc
   :numbered: left
   :practice: T
   :adaptive:

   Create the function, ``incrementing(n)``. Loop while the integer ``n`` is less than 5, and each time through the loop,
   add ``n`` to the list ``new_list`` and then increment ``n`` by 1. Then return the list ``new_list``. For example, 
   if ``n`` is 0, then the function should increment by 1 then return ``[0, 1, 2, 3, 4]``.
   -----
   def incrementing(n):
   =====
       new_list = []
   =====
       while n < 5:
   =====
       while n > 5: #paired
   =====
           new_list.append(n)
           n = n + 1
   =====
       return new_list

.. activecode::  ch5ex1muc-ac

    Write the function, ``incrementing(n)``. Loop while the integer ``n`` is less than 5, and each time through the loop,
    add ``n`` to the list ``new_list`` and then increment ``n`` by 1. Then return the list ``new_list``. For example, 
    if ``n`` is 0, then the function should increment by 1 then return ``[0, 1, 2, 3, 4]``.
    ~~~~
    def incrementing(n):
        # write code here

    ====
    from unittest.gui import TestCaseGui


    class myTests(TestCaseGui):
        def testOne(self):
            self.assertEqual(incrementing(2), [2, 3, 4], 'incrementing(2)')
            self.assertEqual(incrementing(6), [], 'incrementing(6)')
            self.assertEqual(incrementing(4), [4], 'incrementing(4)')
            self.assertEqual(incrementing(0), [0, 1, 2, 3, 4], 'incrementing(0)')

    myTests().main()


.. parsonsprob:: ch5ex2muc
   :numbered: left
   :practice: T
   :adaptive:

   Create the function, ``numbers(accum)``. Loop while the integer ``accum`` is less than 6, and each time through the loop, 
   add ``accum`` to the list, ``new_list`` and then increment ``accum`` by 2. Then return ``new_list``. For example, if ``accum`` 
   is 0, the function should increase its value by 2 and return ``[0, 2, 4]``. 
   -----
   def numbers(accum):
   =====
       new_list = []
   =====
       while accum < 6: 
   =====
       while accum < 7: #paired
   =====
           new_list.append(accum)
           accum = accum + 2
   =====
       return new_list
   


.. activecode::  ch5ex2muc-ac

    Write the function, ``numbers(accum)``. Loop while the integer ``accum`` is less than 6, and each time through the loop, 
    add ``accum`` to the list, ``new_list`` and then increment ``accum`` by 2. Then return ``new_list``. For example, if ``accum`` 
    is 0, the function should increase its value by 2 and return ``[0, 2, 4]``. 
    ~~~~
    def numbers(accum):
        # write code here

    ====
    from unittest.gui import TestCaseGui


    class myTests(TestCaseGui):
        def testOne(self):
            self.assertEqual(numbers(4), [4], 'numbers(4)')
            self.assertEqual(numbers(6), [], 'numbers(6)')
            self.assertEqual(numbers(7), [], 'numbers(7)')
            self.assertEqual(numbers(0), [0, 2, 4], 'numbers(0)')

    myTests().main()


.. parsonsprob:: ch5ex3muc
   :numbered: left
   :practice: T
   :adaptive:

   Create the following function, ``skipCount(start, increment, stop)``. Set ``counter`` to ``start`` and loop while ``counter`` is less than ``stop``
   and each time through the loop, add ``counter`` to the list, ``new_list`` and increment ``counter`` by ``increment``. Then return ``new_list``.
   For example, if ``start`` is 0, ``increment`` is 2, and ``stop`` is 8, the function should increase by 2 and 
   then return ``"[0, 2, 4, 6]"``.
   -----
   def skipCount(start, increment, stop):
   =====
       new_list = []
   =====
       counter = start
   =====
       while counter < stop:
   =====
           new_list.append(counter)
           counter += increment
   =====
       return new_list


.. activecode::  ch5ex3muc-ac

    Write the following function, ``skipCount(start, increment, stop)``. Set ``counter`` to ``start`` and loop while ``counter`` is less than ``stop``
    and each time through the loop, add ``counter`` to the list, ``new_list`` and increment ``counter`` by ``increment``. Then return ``new_list``.
    For example, if ``start`` is 0, ``increment`` is 2, and ``stop`` is 8, the function should increase by 2 and then return ``"[0, 2, 4, 6]"``.
    ~~~~
    def skipCount(start, increment, stop):
        new_list = []
        counter = start

        # write code here

    ====
    from unittest.gui import TestCaseGui


    class myTests(TestCaseGui):
        def testOne(self):
            self.assertEqual(skipCount(0,2,8), [0, 2, 4, 6], 'skipCount(0,2,8)')
            self.assertEqual(skipCount(0,2,9), [0, 2, 4, 6, 8], 'skipCount(0,2,9)')
            self.assertEqual(skipCount(0,2,7), [0, 2, 4, 6], 'skipCount(0,2,7)')

    myTests().main()


.. parsonsprob:: ch5ex4muc
   :numbered: left
   :practice: T
   :adaptive:

   Create the following function, ``loopMe(first, second)``. Loop infinitely while the integer ``first`` is greater than the integer ``second``
   and then return a boolean, ``True``. For example, if ``first`` is 4 and ``second`` is 3, then the function should infintely loop 
   and return ``True``.
   -----
   def loopMe(first, second):
   =====
       while first > second:
   =====
       while first == second: #paired
   =====
           return True
   =====
   loopMe(7, 4)
   =====
   loopMe(1, 3) #paired


.. activecode::  ch5ex4muc-ac

    Write the following function, ``loopMe(first, second)``. Loop infinitely while the integer ``first`` is greater than the integer ``second``
    and then return a boolean, ``True``. For example, if ``first`` is 4 and ``second`` is 3, then the function should infintely loop 
    and return ``True``.
    ~~~~
    def loopMe(first,second):
        # write code here

    ====
    from unittest.gui import TestCaseGui


    class myTests(TestCaseGui):
        def testOne(self):
            self.assertEqual(loopMe(4,3), True, 'loopMe(4,3)')

    myTests().main()


.. parsonsprob:: ch5ex5muc
   :numbered: left
   :practice: T
   :adaptive:

   Create the following function, ``calculation(numbers)``. Using a for loop, add each ``number`` in the list ``numbers`` to ``sum`` and then 
   divide ``sum`` by the length of ``numbers`` to get the average of the list. Then return a float for the average. For example, if ``numbers`` 
   is [90, 94, 85, 78, 87, 98], then the function should return the float 88.66666666666667.
   -----
   def calculation(numbers):
   =====
       sum = 0
   =====
       for number in numbers:
   =====
           sum = sum + number
   =====
           sum = sum - number #paired
   =====
       return sum/len(numbers)

.. activecode::  ch5ex5muc-ac

    Write the following function, ``calculation(numbers)``. Using a for loop, add each ``number`` in the list ``numbers`` to ``sum`` and then 
    divide ``sum`` by the length of ``numbers`` to get the average of the list. Then return a float for the average. For example, if ``numbers`` 
    is [90, 94, 85, 78, 87, 98], then the function should return the float 88.66666666666667.
    ~~~~
    def calculation(numbers):
        sum = 0
        # write code here

    ====
    from unittest.gui import TestCaseGui


    class myTests(TestCaseGui):
        def testOne(self):
            self.assertAlmostEqual(calculation([90, 94, 85, 78, 87, 98]), 88.66666666666667, 2, 'calculation([90, 94, 85, 78, 87, 98])')
            self.assertAlmostEqual(calculation([65, 69, 84, 99, 88, 98]), 83.8333333333333, 2, 'calculation([65, 69, 84, 99, 88, 98])')

    myTests().main()


.. parsonsprob:: ch5ex6muc
   :numbered: left
   :practice: T
   :adaptive:

   Create the following function, ``sum_of_range(start, end)``. Using a for loop, add each ``number`` to the ``sum`` starting from
   ``start`` and going to ``end``. Then return the ``sum``. For example, if ``start`` is 0 and ``end`` is 31, the each ``number`` 
   from 0 to 31 must be added to ``sum`` and return 465.
   -----
   def sum_of_range(start, end):
   =====
       sum = 0
   =====
       for number in range(start, end):
   =====
           sum = sum + number
   =====
           sum = sum + numbers #paired
   =====
       return(sum)


.. activecode::  ch5ex6muc-ac

    Write the following function, ``sum_of_range(start, end)``. Using a for loop, add each ``number`` to the ``sum`` starting from
    ``start`` and going to ``end``. Then return the ``sum``. For example, if ``start`` is 0 and ``end`` is 31, then each ``number`` 
    from 0 to 31 must be added to ``sum`` and return 465.
    ~~~~
    def sum_of_range(start, end):
        sum = 0
        # write code here
    ====
    from unittest.gui import TestCaseGui


    class myTests(TestCaseGui):
        def testOne(self):
            self.assertEqual(sum_of_range(0,31), 465, 'sum_of_range(0,31)')
            self.assertEqual(sum_of_range(0,20), 190, 'sum_of_range(0,20)')
            self.assertEqual(sum_of_range(0,101), 5050, 'sum_of_range(0,101)')

    myTests().main()


.. parsonsprob:: ch5ex7muc
   :numbered: left
   :practice: T
   :adaptive:

   Create the following function, ``odd_sum(start, increment, end)``. Using a for loop, add each ``number`` to the ``sum`` starting from
   ``start`` and going to ``end`` and increment ``start`` with ``increment`` each time. Then return the ``sum``. For example, if ``start`` 
   is 1, ``end`` is 30, and ``increment`` is 2, then each odd ``number`` from 1 to 30 must be added to ``sum`` and return 225.
   -----
   def odd_sum(start, increment, end):
   =====
       sum = 0
   =====
       for number in range(start, end, increment):
   =====
       for numbers in range(start, increment, end): #paired
   =====
           sum = sum + number
   =====
       return sum


.. activecode::  ch5ex7muc-ac

    Write the following function, ``odd_sum(start, increment, end)``. Using a for loop, add each ``number`` to the ``sum`` starting from
    ``start`` and going to ``end`` and increment ``start`` with ``increment`` each time. Then return the ``sum``. For example, if ``start`` 
    is 1, ``end`` is 30, and ``increment`` is 2, then each odd ``number`` from 1 to 30 must be added to ``sum`` and return 225.
    ~~~~
    def odd_sum(start, increment, end):
        sum = 0
        # write code here
    ====
    from unittest.gui import TestCaseGui


    class myTests(TestCaseGui):
        def testOne(self):
            self.assertEqual(odd_sum(1, 2, 30), 225, 'odd_sum(1, 2, 30)')
            self.assertEqual(odd_sum(2, 3, 100), 1650, 'odd_sum(2, 3, 100)')
            self.assertEqual(odd_sum(-1, 4, 30), 104, 'odd_sum(-1, 4, 30)')

    myTests().main()


.. parsonsprob:: ch5ex8muc
   :numbered: left
   :practice: T
   :adaptive:

   Create the following function, ``multiple_three(num)``. Set ``numbers`` to range from 3 to ``num`` that increments by 3 each time.
   Using a for loop, add each ``number`` in ``numbers`` to the ``sum``. Then return the ``sum``. For example, if ``num`` is 37, the function 
   should add every 3rd number from 3 to 37 and return 234.
   -----
   def multiple_three(num):
   =====
       sum = 0
       numbers = range(3, num, 3)
   =====
       for number in numbers:
   =====
           sum = sum + number
   =====
           sum = sum - number #paired
   =====
       return sum

.. activecode::  ch5ex8muc-ac

    Write the following function, ``multiple_three(num)``. Set ``numbers`` to range from 3 to ``num`` that increments by 3 each time.
    Using a for loop, add each ``number`` in ``numbers`` to the ``sum``. Then return the ``sum``. For example, if ``num`` is 37, the function 
    should add every 3rd number from 3 to 37 and return 234.
    ~~~~
    def multiple_three(num):
        sum = 0
        # write code here
    ====
    from unittest.gui import TestCaseGui


    class myTests(TestCaseGui):
        def testOne(self):
            self.assertEqual(multiple_three(37), 234, 'multiple_three(37)')
            self.assertEqual(multiple_three(101), 1683, 'multiple_three(101)')
            self.assertEqual(multiple_three(19), 63, 'multiple_three(19)')

    myTests().main()

.. parsonsprob:: ch5ex9muc
   :numbered: left
   :practice: T
   :adaptive:

   Create the following function, ``water_quality(pHvalues)``. Using a for loop, add each ``pH`` in the list ``pHvalues`` to ``total`` and then
   divide ``total`` by the length of ``pHvalues`` to get the average of the list. Then return a float for the average. For example, if ``pHvalues`` 
   is [7.0, 8.2, 6.7, 7.5, 8.0, 7.2], then the function should return 7.433333333333334.
   -----
   def water_quality(pHvalues):
   =====
       total = 0 
   =====
       for pH in pHvalues:
   =====
           total = total + pH
   =====
           total = total * pH #paired
   =====
       average = total / len(pHvalues)
   =====
       return average

.. activecode::  ch5ex9muc-ac

    Write the following function, ``water_quality(pHvalues)``. Using a for loop, add each ``pH`` in the list ``pHvalues`` to ``total`` and then
    divide ``total`` by the length of ``pHvalues`` to get the average of the list. Then return a float for the average. For example, if ``pHvalues`` 
    is [7.0, 8.2, 6.7, 7.5, 8.0, 7.2], then the function should return 7.433333333333334.
    ~~~~
    def water_quality(pHvalues):
        total = 0 
        # write code here
    ====
    from unittest.gui import TestCaseGui


    class myTests(TestCaseGui):
        def testOne(self):
            self.assertAlmostEqual(water_quality([7.0, 8.2, 6.7, 7.5, 8.0, 7.2]), 7.433333333333334, 2, 'water_quality([7.0, 8.2, 6.7, 7.5, 8.0, 7.2], 6)')
            self.assertAlmostEqual(water_quality([7, 8, 6, 7, 8, 7]), 7.166666666667, 2, 'water_quality([7, 8, 6, 7, 8, 7])')
  

    myTests().main()


.. parsonsprob:: ch5ex10muc
   :numbered: left
   :practice: T
   :adaptive:

   Create the following function, ``countdown(counter)``. Loop while ``counter`` is greater than 0 and each time through the loop,
   add ``counter`` to the list ``new_list`` and then decrement ``counter`` by 1. Then return ``new_list``. For example, if ``counter`` 
   is 5, then the function should countdown from 5 and return ``[5, 4, 3, 2, 1]``.
   -----
   def countdown(counter):
   =====
       new_list = []
   =====
       while counter > 0:
   =====
           new_list.append(counter)
   =====
           counter = counter - 1
   =====
           counter = counter + 1 #paired
   =====
       return new_list


.. activecode::  ch5ex10muc-ac

    Write the following function, ``countdown(counter)``. Loop while ``counter`` is greater than 0 and each time through the loop,
    add ``counter`` to the list ``new_list`` and then decrement ``counter`` by 1. Then return ``new_list``. For example, if ``counter`` 
    is 5, then the function should countdown from 5 and return ``[5, 4, 3, 2, 1]``.
    ~~~~
    def countdown(counter):
        # write code here
    ====
    from unittest.gui import TestCaseGui


    class myTests(TestCaseGui):
        def testOne(self):
            self.assertEqual(countdown(5), [5, 4, 3, 2, 1], 'countdown(5)')
            self.assertEqual(countdown(3), [3, 2, 1], 'countdown(3)')
            self.assertEqual(countdown(7), [7, 6, 5, 4, 3, 2, 1], 'countdown(7)')
            self.assertEqual(countdown(-1), [], 'countdown(-1)')

    myTests().main()
