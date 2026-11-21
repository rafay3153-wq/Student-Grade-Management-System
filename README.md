Student Grade Management System

A command-line Python program that records subject marks for a student and produces a per-subject grade report along with an overall summary (total marks, percentage, grade, and average GPA).

Authors
Shehryar Khurram (FA25-BDS-045)
Muhammad Rafay (FA25-BDS-035)

COMSATS University Islamabad

Features
Collects student name, roll number, and number of subjects
Validates all numeric input (re-prompts on invalid or out-of-range values)
Calculates percentage, letter grade, and GPA for each subject
Prints a formatted results table
Prints an overall summary: total marks, overall percentage, overall grade, and average GPA
Requirements
Python 3.6 or later (uses f-strings)
How to Run
bash
python main.py

Replace main.py with the name of your file.

Usage
Enter the student's name and roll number.
Enter the number of subjects (must be a positive integer).
For each subject, enter the subject name, total marks, and obtained marks (between 0 and the total).
The program prints the results table and the overall summary.
Grading Scale
Percentage	Grade	GPA
85 and above	A	4.0
80 - 84	A-	3.7
75 - 79	B+	3.3
70 - 74	B	3.0
65 - 69	B-	2.7
60 - 64	C+	2.3
55 - 59	C	2.0
50 - 54	C-	1.7
45 - 49	D	1.0
Below 45	F	0.0

The overall grade is based on the overall percentage. The average GPA is the mean of the per-subject GPAs.

Code Structure
Function	Purpose
get_positive_int(msg)	Prompts until the user enters an integer greater than 0.
get_marks(mssg, total_marks)	Prompts until the user enters a number between 0 and the subject's total marks.
calculate_grade(percent)	Maps a percentage to a letter grade and GPA.
main()	Runs the program: input, calculation, and report output.
Example Output
Subject         Total      Obtained     Percentage   Grade    GPA
===================================================================
Maths           100        82           82.00        A-       3.7
Physics         100        68           68.00        B-       2.7

==================== OVERALL SUMMARY ====================
Total Obtained Marks : 150.0 / 200
Overall Percentage   : 75.00%
Overall Grade        : B+
Average GPA          : 3.20
==========================================================
Concepts Practiced
Functions and return values (including tuples)
Input validation with while True and try / except
Lists to store per-subject data
for loops and range()
Formatted output with f-strings and str.format()
