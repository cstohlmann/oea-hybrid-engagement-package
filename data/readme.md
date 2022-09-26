# Data Dependencies

This package combines multiple data sources which were identified through answering concepts surrounding hybrid student engagement:

* <strong>School Information System (SIS)</strong>: School, grade level, class roster, and demographics.
* <strong>Attendance data</strong>: Student in-person attendance data.
* <strong>Digital Engagement data</strong>: Application use, type of engagement (log-ins, Teams meeting attendance duration, etc.), date of the activity, and user information of the activities.

## Attendance Data

Gathering data pertaining to student (in-school or outside-of-school) attendance is necessary for developing sufficient analysis in hybrid student engagement. Understanding the distibution of student in and out of school attendance, grants administration the ability to see how either forms of student attendance directly affects student learning. 

For this package we used the [Contoso SIS studentattendance table](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/module_catalog/Student_and_School_Data_Systems) as our source of fictitious test data for the records of in-person student attendance.

## Digital Engagement Data

In order to better understand hybrid student engagement in an education system, collecting and analyzing forms of digital engagement is significant. This can provide education system leaders with data to identify patterns of frequent engagement or unengagement in certain applications. These emergent patterns of engagement can provide a segway to analyze how different methods of engagement impact student learning outcomes. 

* **M365 [Education Insights](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/module_catalog/Microsoft_Education_Insights)**: Digital activity related to M365 applications
* **[Clever](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/module_catalog/Clever)**: Learning app activity
* **[i-Ready](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/module_catalog/iReady)**: Math and english learning activity

## Power BI Data Model

<strong><em>[All of this needs to be changed and updated.]</strong></em>

Below is a view of the data model used in Power BI visualizations. The primary tables and relationships can be seen.

* **studentPBI Table**: Most of the SIS data is contained within this table - data on student demographics, school they attend, etc.
* **myqoiPBI Table**: Time dependent records of student access/connectivity data.
* **studentsection Table**: Contains section SIS data - the class(es) that students are a part of.
* **destiny Table**: Data used to relay student device assignment by the education system.
* **school_locations Table**: Data used to create maps of school locations. 

![](https://github.com/cviddenKwantum/oea-digital-learning-insights/blob/main/Digital_Equity_of_Access/docs/images/pbi_datamodel.png)
