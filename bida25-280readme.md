THE GRADEBOOK  MANAGEMENT SYSTEM  ASSIGNMENT

Section A:  Initial Setup  - Scalar  Objects and  Loops  
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
