## Purpose of the VA
The focus of our visual analytics system is absenteeism within western Mass counties. We were asked by 
members of the Public Health Institute of Western MA to create a public facing system that can visualize 
the trends per county. We are looking at absenteeism from multiple different angles, namely attendance rate, 
average number of absences, chronically absent, and the overall trends. Chronically absent is defined as missing 
at least 10% of the total school days for that year. The attendance rate was first broken down to each individual 
school, but we later created an attendance rate for each county for each year. The average number of absences was 
found by taking the number of students who had over nine unexcused absences by the end of the year and divided 
it by the total enrolled for that school. Our VA system is meant to show the problem of absenteeism in schools. 
The Public Health Institute wants this data to be able to show the problems with students missing school and try
and the effects it has. Absenteeism is a problem that is not highlighted enough but it is extremely important. The hope
is to improve absenteeism moving forward, especially after the COVID-19 pandemic. This dashboard is the first step in 
creating more awareness and action taken to keep kids in school. 



## How to Use 







## Any bugs 







## Dataset Cleaning Methods

Each Tableau Visualization will have a cleaned dataset created by joining the Absenteeism dataset and School Size/County dataset provided by stakeholder Sinead Keogh. 

The cleaned datasets will be obtained through R Code and the cleaning steps taken will be documented through comments.

Datasets Used:
- Absenteeism Dataset: https://profiles.doe.mass.edu/statereport/attendance.aspx
- School Size/County Dataset: https://www.doe.mass.edu/infoservices/reports/enroll/default.html?yr=2425
