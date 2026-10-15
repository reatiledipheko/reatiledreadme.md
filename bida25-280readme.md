THE  GRADEBOOK  MANAGEMENT  SYSTEM  ASSIGNMENT

Section  A:  Initial  Setup  -  Scalar  Objects  and  Loops  
This is the initial setup of the system which handles the basic input and output operations. It works with Scalar objects such as integers, for loops like "while".
The scetions collects student names and grades, calculates the class averages as will as printing a students report.

The code satisfies:
-Asking the user how many students there are
-Collects data: a for loop that runs once per students, asking for their name with a while loop that asks for their grade and checks that the grade is between 0 and 100.
-It calculates through all students and adds uo the grades (student[1]) into the total. Calculates the average=total/num_students.

The Concepts Used
-Lists and nested lists
-For and while loops
-Input validation with if/else
-Input() and type conversion

Section  B:  Expanding  with  Lists  and  Tuples  
This part of the system collects grades for multiple students across the three subjects we have, then reports each students average alongside the highest and lowest per subject and a summary table.

It satisfies:
-A list of subjects
-Asking the user how many students there are (students_num)
-Collects data: a for loop that runs once per student and prints the student number, nested loop that goes through each subjects and asks for a grade and a while loop that keeps asking until the grade 
is between 0 and 100.
-Loops through students and calculates sum(grades) / len(grades).
-Loops through each subject by its index i 
-Contains a summary table

The Concepts Used
-Lists, tuples and nested data
-for loops, nested and while loops
-Input validation
-List comprehensions
-sum(),len(),max(),min(), and round()
-string formating with ljust() and rjust(). This are pad strings with spaces so it reaches a set width.

Section  C:  Introduction  of  Dictionaries  
Stores student grades in nested dictionaries. Users can add, update and remove students,view grades by subject,search for a students aand see a summary table.

It satisfies:
-a while loop which keeps showing the menu until the user chooses Exit and each menu option calls its own function.
-asks for grade and keeps asking until the input is 0 and 100
-shows the avaliable subjects and asks the user to pick one.
-collects every grade across all subjects for one students and returns the average.

Concepts used
-Nested Dictionaries and lists
-Functions with return values
-While loops and menu-driven programs
-Try/except error handling
-Input validation

Section D: 



