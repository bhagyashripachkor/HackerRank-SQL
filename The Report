You are given two tables: Students and Grades. Students contains three columns ID, Name and Marks.

Grades contains the following data:grade min_marks max_marks

Ketty gives Eve a task to generate a report containing three columns:  Name, Grade and Mark. 
Ketty doesn't want the NAMES of those students who received a grade lower than 8. 
The report must be in descending order by grade -- i.e. higher grades are entered first. 
If there is more than one student with the same grade (1-10) assigned to them, order those particular students by their name alphabetically. 
Finally, if the grade is lower than 8, use "NULL" as their name and list them by their marks in ascending order.

Write a query to help Eve.

SELECT 
CASE WHEN grd.grade < 8 THEN NULL 
WHEN grd.grade >= 8 THEN std.name END,
grd.grade, std.marks FROM students std, grades grd
WHERE std.marks BETWEEN grd.min_mark AND grd.max_mark
ORDER BY grd.grade DESC, std.name ASC;
