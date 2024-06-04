// INNER JOIN

SELECT students.id, students.name, courses.course
FROM students
INNER JOIN courses ON students.course_id = courses.id;


//LEFT JOIN

SELECT students.id, students.name, courses.course
FROM students
LEFT JOIN courses ON students.course_id = courses.id;


//RIGHT JOIN

SELECT students.id, students.name, courses.course
FROM students
RIGHT JOIN courses ON students.course_id = courses.id;

// FULL OUTER JOIN

SELECT students.id, students.name, courses.course
FROM students
LEFT JOIN courses ON students.course_id = courses.id
UNION
SELECT students.id, students.name, courses.course
FROM students
RIGHT JOIN courses ON students.course_id = courses.id;



