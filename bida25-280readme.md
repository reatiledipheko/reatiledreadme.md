THE GRADEBOOK  MANAGEMENT SYSTEM  ASSIGNMENT

Section A: 
Initial Setup  - Scalar  Objects and  Loops  
This is the student grade report that asks how many students there are, collects each student's name and grade, then 
calculates the class average and prints a student report. Each student is stored as a small list with two items: [name, grade].
All the students go inside one bigger list called students. The code works in a way that it creates  an empty list called students 
and asks how many students there are.Collects data on a for loop thats runs once for each student. For each one it:

-Prints the student number
-Asks for the name
-Asks for the grade

It checks the grade with a while True loop that keeps asking until the grade is between 0 and 100.If the grade is valid, break stops the loop.
If it is not valid, an error message shows and the program asks again plus the student as students.append([name, grade]) adds the student to the list.
The system calculates the average with another loop adds up every grade into total. Then average = total / student_num. If there are no students,the average
is set to 0 so the program doesn't divide by zero.It prints ===STUDENT REPORT===, then loops through the list and prints each student's name and grade.

What I Used In Section
-Lists and lists inside lists
-for loops and while loops
-if / else
-input(), int() and float()
-append() and break

Section B:
Student Grade Analysis
This program collects grades for several students in three subjects (Math, English and Science). It then shows each student's average, the highest and
lowest grade in each subject, and a summary table. The code works in way that it makes the subjects list, an empty students list, and asks how many students 
there are. It collects data in a for loop for each student, it asks for the name, a second for loop goes through each subject and asks for grade, a while
loop keeps asking if the grade is below 0 or above 100 and the student is saved as (name, grades). for each student. Additionally, for each student, sum(grades) / len(grades)
gives the average. It is rounded to 1 decimal place with the highest and lowest per subject for each subject the program collects every student's grade for that subject into a list,
then uses max() and min() to find the highest and lowest and a summary table that builds a header row and a row for each student. ljust() and rjust() add spaces so the columns line up.
The program collects every student's grade for that subject into a list, then uses max() and min() to find the highest and lowest. 

What ljust() and rjust() do:
-ljust(12) puts the text on the left and adds spaces after it, until it is 12 characters wide.
-rjust(10) puts the text on the right and adds spaces before it, until it is 10 characters wide

What I used:
-Lists and tuples
-for loops (including a loop inside a loop) and while loops
-List comprehension: [grades[i] for name, grades in students]
-sum(), len(), max(), min() and round()
-ljust() and rjust()

Section C: 
Student Grade Manager (Dictionaries)

This program manages student grades using dictionaries. The user picks an option from a menu to add, update, remove or search for students, or to view all the grades for one subject.
A dictionary stores data in key: value pairs, like a real dictionary where a word (the key) has a meaning (the value).In this program: The key is the student's name and the value is 
another dictionary with the student's subjects and grades. How the code works: the menu sits inside a while True loop, so it keeps showing until the user chooses 6. Exit. An if / elif 
chain checks which option was chosen. 

What it does
1. Add a student	Asks for a name. If the student already exists it says so. Otherwise it asks for a grade in each subject and saves them.
2. Update a student's grades	Finds the student and subject, shows the current grades, then the user types A to add a grade or R to replace all grades.
3. Remove a student	Asks for a name and deletes that student with del.
4. View all grades for a subject	Asks for a subject and prints every student's grades for it.
5. Search for a student	Prints one student's grades and works out their average.
6. Exit	Prints "Goodbye!" and uses break to stop the loop.

How the average is worked out the program goes through every grade for the student. It adds each one to total and adds 1 to count. Then average = total / count.

What I used
-Dictionaries, including a dictionary inside a dictionary
-Lists and .append()
-while loops and for loops
-if / elif / else
-del to remove from a dictionary

Section D: 
Student Grade Manager (Functions)
This is the section C program, but the code is now split into functions. The user picks an option from a menu to add, search, update, display or remove students.
The program also checks for errors, so it doesn't crash when something goes wrong. A function is a named block of code that does one job. You write it once with def,
then use it ("call" it) whenever you need it by writing its name with brackets, like add student(). Functions make the code easier to read, easier to fix, and let you 
reuse the same code in many places.

The Functions

get_grade(subject):Asks for one grade and repeats until it is a number from 0 to 100. Gives the grade back with return.
calculate_average(record):Adds up all of one student's grades and divides by how many there are.
add_student():Asks for a name, checks it is not empty or already used, then collects a grade for each subject.
display_student(name):Prints one student's grades and average.
display_summary():Prints every student's grades and average.
search_and_update():Finds a student by name, shows them, then lets the user add a grade or replace the grades in a subject.
remove_student():Deletes a student.
view_subject():Prints every student's grades for one subject.
main():Shows the menu and calls the other functions.

Error handling with try/except
Python runs the code under try. If an error happens, it jumps to except instead of crashing.

ValueError:	The user types letters instead of a number for a grade the program shows an error and asks again
KeyError:	The student's name is not in the dictionary and	shows "student not found"
ZeroDivisionError:	A student has no grades to average and shows an error and returns 0

What I used
Functions with def, parameters and return
Dictionaries and lists
try / except
while loops, for loops and if / elif / else

Section E and F

The Gradebook Management System is a Python-based application developed using Object-Oriented Programming (OOP) principles. The system allows users to manage student records, store grades, calculate averages, search for students, remove students, and sort student data.

This project demonstrates the use of classes, objects, methods, encapsulation, exception handling, and input validation.

Objectives

The main objectives of this project are:

Implement Object-Oriented Programming concepts.
Create and manage student records.
Store and maintain student grades.
Calculate average grades automatically.
Search and remove student records.
Sort students by average grade or subject grade.
Handle user input errors effectively.

Features
Student Management
Add new students.
Prevent duplicate student records.
Search for existing students.
Remove students from the system.

Grade Management
Add grades for different subjects.
Store multiple subject grades for each student.
Calculate average grades automatically.

Sorting Functions
Sort students by overall average grade.
Sort students by specific subject grades.

Input Validation
Prevent empty student names.
Prevent empty subject names.
Validate grade values between 0 and 100.
Handle invalid inputs using exception handling.

Object-Oriented Design
Student Class

The Student class represents an individual student.

Attributes
name
grades

Methods
Method	Descriptionadd_grade()	-Adds a subject and grade
calculate_average()             -	Calculates the average grade
print_details()	                -Displays student information


