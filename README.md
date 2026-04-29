## Purpose of the VA
The focus of our visual analytics system is absenteeism within western Mass counties. We were asked by 
members of the Public Health Institute of Western MA to create a public facing system that can visualize 
the trends per county. We are looking at absenteeism from multiple different angles, namely attendance rate, 
average number of absences, chronically absent, and the overall trends. Chronically absent is defined as missing 
at least 10% of the total school days for that year. The attendance rate was first broken down to each individual 
school, but we later created an attendance rate for each county for each year. The average number of absences was 
found by taking the number of students who had over nine unexcused absences by the end of the year and divided 
it by the total enrolled for that school. 

Our VA system is meant to show the problem of absenteeism in schools in a way that is easy for the public to understand. To support this, the dashboard uses three different visual encodings: color to compare counties, line positions to show changes over time, and length of bars to compare absenteeism values across counties. The VA system also includes details-on-demand interaction, allowing users to click or hover over parts of the dashboard to see more specific information or value for a specific year. In addition, the dashboard uses a coordinated view of data, meaning that multiple graphs work together so users can compare absenteeism patterns across counties, years, and indicators.
 
The Public Health Institute wants this data to be able to show the problems with students missing school and try
and the effects it has. Absenteeism is a problem that is not highlighted enough but it is extremely important. The hope
is to improve absenteeism moving forward, especially after the COVID-19 pandemic. This dashboard is the first step in 
creating more awareness and action taken to keep kids in school. 



## How to Use 

This dashboard explores absenteeism trends in Western Massachusetts counties from 2017 to 2025, focusing on three key metrics: average attendance rate, 10% chronic absenteeism, and average number of absences. Use the tabs at the top to navigate between views.

### 1. Overview Tab

The Overview tab gives users a summary of the main attendance and absenteeism patterns across Western Massachusetts counties. It combines a trend line graph with three county-level bar charts, so users can see both changes over time and county comparisons for a selected school year.

#### Main features

- The line graph at the top shows changes over school years.
- The drop-down menu allows users to switch the variable displayed in the line graph.
- The bar charts below show county-level average values for:
  - Attendance Rate
  - 10% Chronic Absenteeism
  - Average Number of Absences
- A text label shows which school year the bar charts are currently displaying.

#### How to interact with this tab

- Use the drop-down menu to choose the variable shown in the line graph.
- Hover over points on the line graph to see detailed information, including county, school year, variable, and weighted average value.
- Click a point on the line graph to update the bar charts to that school year and highlight the selected county in the bar charts.
- Use the bar charts to compare counties for the selected school year.

### 2. Overtime Trends Tab

The Overtime Trends tab focuses on changes across school years. It allows users to compare county-level trends for one selected variable at a time.

#### Main features

- The line graph shows county-level trends from 2017-18 to 2024-25.
- Each line represents one county.
- The color legend identifies the county represented by each line.
- The variable drop-down menu allows users to switch between different measures.

#### How to interact with this tab

- Use the variable drop-down menu to select the variable you want to explore.
- Hover over a point on a line to see details, including county, school year, variable, and weighted average value.
- Click a line to highlight one county and make it easier to follow its trend over time.

### 3. Attendance Rate Tab

The Attendance Rate tab shows the average attendance rate for each county in a selected school year. Users can use this tab to compare county-level attendance rates and identify which counties had higher or lower attendance rate during that year.

#### Main features

- Each horizontal bar represents one county.
- The value label at the end of each bar shows the average attendance rate as a percentage.
- The school-year slider allows users to select a specific school year.

#### How to interact with this tab

- Drag the school-year slider to choose a school year.
- Hover over a bar to see details, including county, school year, and average attendance rate.
- Click a bar to highlight that county.
- Compare the bar lengths and percentage labels to see which counties had higher or lower attendance rates in the selected year.

### 4. 10% Chronic Absenteeism

The 10% Chronic Absenteeism tab shows the percentage of students who were absent for 10% or more of their total membership days by county for a selected school year.

#### Main Features:
- The bar chart shows the county-level average 10% chronic absenteeism rate for the selected school year.
- Each bar represents one county, with longer bars indicating higher chronic absenteeism rates.
- Values are displayed as percentages at the end of each bar.
- Lower percentages indicate fewer students with significant absences.
- This measure includes students in grades PK–12 with at least 20 days of membership.

#### How to Interact:
- Hover over a bar to see the county, school year, and chronic absenteeism rate.
- Click a bar to highlight it.
- Drag the school-year slider on the right to select a specific school year between 2017 and 2025.

### 5. Average # Absences

The Average # Absences tab shows the average number of absences by county for a selected school year.

#### Main Features:
- The bar chart shows the average number of absences for each county in the selected school year.
- Each bar represents one county, with longer bars indicating a higher average number of absences.
- Values are displayed at the end of each bar.
- Lower values indicate fewer average absences.

#### How to Interact:
- Hover over a bar to see the county, school year, and average number of absences.
- Click a bar to highlight it.
- Drag the school-year slider on the right to select a specific school year between 2017 and 2025.


## Any bugs 

For the overtime trends line graph in the overview tab, choosing a specific dot on a line is slighltly difficult. This is because the dots are small, and there are dots from other lines displaying at the same time so it's easy to misclick the dots on the other lines. 

Also in the overview tab, if the users double click on one of the county in one of the bar graphs, the other bars in this graph will disappear without any instruction on how to bring them back. 

For the attendance rate variable in the overtime trends line graph, the county lines overlapped a bit too much because the y-axis range from 0 to 100 percent but most of the lines are around the 90 to 100 percent range. So this might be hard to visually identify the difference in attendance rate for different counties. 



## Dataset Cleaning Methods

Each Tableau Visualization will have a cleaned dataset created by joining the Absenteeism dataset and School Size/County dataset provided by stakeholder Sinead Keogh. 

The cleaned datasets will be obtained through R Code and the cleaning steps taken will be documented through comments.

Datasets Used:
- Absenteeism Dataset: https://profiles.doe.mass.edu/statereport/attendance.aspx
- School Size/County Dataset: https://www.doe.mass.edu/infoservices/reports/enroll/default.html?yr=2425
