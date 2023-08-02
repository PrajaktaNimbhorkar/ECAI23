# ECAI23
ECAI 2023 code and data
This dataset contains the data from the Student Elective Allocation Tool, used to allocate courses to engineering students at the Indian Institute of Technology, Madras (IITM). All engineering students at IITM are required to complete a certain number of Humanities and Mathematics courses as part of their curriculum. As such, every semester sees a large number of students applying to courses that interest them, and the matching process can be viewed as a matchings with preferences problem.

We only report the preferences that the students indicated on the application tool, not the results of the matching process. For privacy reasons, all data is anonymized. We report the data from 3 separate semesters.

anon_courses.csv contains the course names and their maximum capacity. The first column is the course number. Course numbers starting with an 'M' are mathematics courses and course numbers starting with an 'H' are humanities courses. The 3 digit number following the first letter is a unique identifier for the course. The second column contains the maximum capacity of the corresponding course.


anon_studentPreferences.csv contains the preference lists of the students. The first column contains the student roll number (a unique identifier for the students) and the following columns indicate the corresponding student's preferences over the courses.

Student roll numbers have the following format - D__B____. The numbers following the "D" indicate which department (i.e. major) the student is enrolled in. At the time of collection of this dataset, students at IITM did not have the option to double-major, and students joined the programme with an assigned major starting from their first year. The number following the "B" is a 4 digit unique identifier. The first digit of the identifier correlates to their year of study : if two students have the same digit, then they are in the same year of study.

For example, consider two students with roll numbers D01B1001 and D02B1023. They are enrolled in different departments but are in the same year of study. Conversely, students D13B2001 and D13B3001 are enrolled in the same department but are in different years of study.
