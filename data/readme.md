# Data Dependencies

This package combines multiple data sources which were identified through answering concepts surrounding hybrid student engagement:

* **School Information System (SIS)**: Student school, grade, roster, and demographics data.
* **Digital Engagement data**: Resource usage (e.g. website visits, application use), lesson completion results, Microsoft application usage. 
* **Attendance data**: Student in-person and/or digital attendance.
* **Learning Outcomes data**: Diagnostic assessment results, student letter-grade assignment.

## Digital Engagement Data

In order to better understand hybrid student engagement in an education system, collecting and analyzing forms of digital engagement is significant. This can provide education system leaders with data to identify patterns of frequent engagement or unengagement in certain applications. These emergent patterns of engagement can provide a segway to analyze how different methods of engagement impact student learning outcomes. 

## Attendance Data

Gathering data pertaining to student (in-school or outside-of-school) attendance is necessary for developing sufficient analysis in hybrid student engagement. Understanding the distibution of student in and out of school attendance, grants administration the ability to see how either forms of student attendance directly affects student learning. 

## Learning Outcomes Data

Learning outcomes data gives benchmarkers and indicators of the results seen from student engagement. This could come from the speed at which students complete lesson material with passing results from i-Ready data, or understanding the distribution of in versus out of school attendance affects student performance on diagnostic assessments. 

## Power BI Data Model

<strong><em>[All of this needs to be changed and updated.]</strong></em>

Below is a view of the data model used in Power BI visualizations. The primary tables and relationships can be seen.
* **studentPBI Table**: Most of the SIS data is contained within this table - data on student demographics, school they attend, etc.
* **myqoiPBI Table**: Time dependent records of student access/connectivity data.
* **studentsection Table**: Contains section SIS data - the class(es) that students are a part of.
* **destiny Table**: Data used to relay student device assignment by the education system.
* **school_locations Table**: Data used to create maps of school locations. 

![](https://github.com/cviddenKwantum/oea-digital-learning-insights/blob/main/Digital_Equity_of_Access/docs/images/pbi_datamodel.png)
