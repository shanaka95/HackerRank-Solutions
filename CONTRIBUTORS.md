Add your solutions for Hackerrank problems.<br>

Your program file name should be equal to Hackerrank problem name and you should add your programming languageto end of name.
<br><br>
Example: Sample_challange_python2

<br><br>you can add more than one solution to a problem.But please dont add wrong solutions.

<br>Your Solution file should be in below structure<br><br>

Example: <br><br>

HackerLand University has the following grading policy:<br>

    Every student receives a in the inclusive range from to .
    Any less than is a failing grade.

Sam is a professor at the university and likes to round each student's according to these rules:<br>

    If the difference between the and the next multiple of is less than , round up to the next multiple of .<br>
    If the value of is less than , no rounding occurs as the result will still be a failing grade.<br>

For example, will be rounded to but will not be rounded because the rounding would result in a number that is less than .<br>

Given the initial value of for each of Sam's students, write code to automate the rounding process. For each , round it according to the rules above and print the result on a new line.<br>
<br><br>
Input Format<br><br>

The first line contains a single integer denoting (the number of students).<br>
Each line of the subsequent lines contains a single integer, , denoting student 's grade.<br>
<br>

Output Format<br><br>

For each of the grades, print the rounded grade on a new line.<br>

Sample Input 0<br>

4<br>
73<br>
67<br>
38<br>
33<br>
<br>
Sample Output 0<br>
<br>
75<br>
67<br>
40<br>
33<br>
<br>
Explanation 0<br>
<br>

<br>
    Student received a , and the next multiple of from is . Since , the student's grade is rounded to .<br>
    Student received a , and the next multiple of from is . Since , the grade will not be modified and the student's final grade is .<br>
    Student received a , and the next multiple of from is . Since , the student's grade will be rounded to .<br>
    Student received a grade below , so the grade will not be modified and the student's final grade is .<br>

<br><br>

Solution:<br><br>
<br><br>

for i in xrange(input()):
    mark=input()
    if mark<38:
        print mark
    elif mark%5>2:
        print mark+(5-mark%5)
    else:
        print mark


