Mixed-Up Code Exercises
------------------------
.. parsonsprob:: inheritance_mixedupcode_1
    :numbered: left
    :practice: T
    :adaptive:

   Create a class ``Parent`` to have their eye_color be hazel. Next, write the class, Child, which is a subclass of Parent to 
   inherit the eye_color of the Parent using the object lil_child.
   ----
   class Parent:
   =====
   class Parent #paired
   =====
     def eye_color(self):
   =====
        return "I have hazel eyes."
   =====
   class Child(Parent):
   =====
   class Child(): #paired
   =====
     def eye_color(self):
   =====
        super().eye_color()
   =====
   lil_child = Child()

..activecode:: inheritance_mixedupcode_1-ac

   Write a class ``Parent`` to have their eye_color be hazel. Next, write the class, Child, which is a subclass of Parent to 
   inherit the eye_color of the Parent using the object lil_child.
   
   ----
   class Parent:
        # write code here
  
  
   class Child:
        # write code here
      
   ====
   from unittest.gui import TestCaseGui

   class myTests(TestCaseGui):
       def testOne(self):
           self.assertEqual(lil_child.eye_color(), "I have hazel eyes")

   myTests().main()