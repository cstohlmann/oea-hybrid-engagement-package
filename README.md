# Hybrid Student Engagement Package

The OEA Hybrid Student Engagement Package provides a set of assets which support an education system in developing their own holistic model to address and gauge hybrid student engagement. There are two main components of this package: 

1. <ins>Guidance and documentation:</ins> The [OEA Hybrid Student Engagement Package - Use Case Documentation]() provides guidance on the end-to-end process of developing a successful Hybrid Student Engagement use case project, including how to engage stakeholders in the project, prior research on the use case problem domain and theory, how to map data sources to the theory of the problem, and how to implement Microsoft’s Principles of Responsible Data and AI. <em> It is highly recommended this document be reviewed by any education system considering using this package, and that the documentation be revised to the specific data and decisions for that system’s context.  </em>
2. <ins>Technical assets:</ins> Various assets are freely available in this package to help accelerate implementation of Hybrid Student Engagement use cases. Assets include descriptions of data sources, notebooks for data processing, a pipeline for model building and deployment, and sample PowerBI dashboards. See descriptions of technical assets below.

This OEA Package was developed through a partnership between Microsoft Education and [Kwantum Analytics](https://www.kwantumedu.com/).

## Problem Statement

Student engagement in learning is the starting point for teaching and learning outcomes. Without engagement, learning is blocked. 

As teaching and learning increasingly use digital platforms and tools, and learning takes place outside of schools in digital learning environments, traditional attendance measures are not as representative of students’ actual engagement. Student attendance data is an important metric that schools track and derive insights from. Schools also need a way to measure students' digital activity across the different apps used for learning. With many schools’ transition to hybrid learning, having a way to combine students' in-person attendance in schools and their digital activity will be valuable for school systems. This combination provides a more comprehensive view of student engagement in learning than attendance data alone.

This package is intended for the use of education systems seeking to better understand the impact of numerous forms of student engagement on student learning outcomes. Forms of engagement can include data on student in-person attendance, student digital attendance, to student application/website uses. Microsoft Education and [Kwantum Analytics](https://www.kwantumedu.com/) collaborated to create an open source GitHub module on [Open Education Analytics (OEA)](https://openeducationanalytics.org/) to enable education systems to use their data effectively to see the various levels of hybrid student engagement for learning, so that they can ensure student successes, in and out of the classroom.

## Package Impact

This use case resulted in a data dashboard that shows patterns of student engagement, while identifying which students are academically struggling - and emerging patterns with lack of engagement implications on student struggle. This OEA package can be used by system and school leaders, and by teachers to identify:
 - Which schools and classes have higher and lower levels of hybrid engagement in learning, and whether expected patterns of engagement are continuing over time. 
 - Which schools and classes have higher and lower levels of in-person attendance or digital activities. This can be used to plan more precisely targeted programs or interventions to increase either attendance or use of digital learning tools, or both. 

The assets in this package can be combined with course completion, academic assessments, competency measures, mastery data, graduation rates, or other outcome data to identify how patterns of engagement relate to learning outcomes. With such combined data, schools and teachers can start to analyze whether new programs or interventions help to improve learning outcomes.  

See below for examples of developed PowerBI dashboards (see also [Power BI]()).

<strong><em>[NEEDS TO BE UPDATED]</strong></em>
Equity of Digital Access  | Quality of Digital Access
:-------------------------:|:-------------------------:
![](https://github.com/cviddenKwantum/oea-digital-learning-insights/blob/main/Digital_Equity_of_Access/docs/images/pbi1nosignal.png) |  ![](https://github.com/cviddenKwantum/oea-digital-learning-insights/blob/main/Digital_Equity_of_Access/docs/images/pbi2landscape.png)

## Data Sources

This package combines multiple data sources which were identified through evaluating the characteristics of digital equity: 
* <strong>School Information System (SIS)</strong>: School, grade level, class roster, and demographics
* <strong>Access/Connectivity data</strong>: Upload and download speed, latency, request processing time, internet provided
* <strong>Device Assignment data</strong>: Device information, student assignment

This package can use several [OEA Modules](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules) to help ingest data sources that are typically used to understand patterns of digital inequity (see below for list of relevant OEA modules).  

| OEA Module | Description |
| --- | --- |
| [Ed-Fi Data Standards](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Education_Data_Standards/Ed-Fi) | For typical Student Information System (SIS) data, including school rosters, grade level and demographic information. |
| [Microsoft Education Insights](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Microsoft_Data/Microsoft_Education_Insights) | For Microsoft engagement/activity data. |
| [Microsoft Graph](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Microsoft_Data/Microsoft_Graph) | For other forms of Microsoft engagement/activity data. |
| [Clever](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Digital_Learning_Apps_and_Platforms/Clever) | For engagement/activity data pertaining to student use of digital learning applications, used and managed by an education system. |
| [i-Ready](https://github.com/microsoft/OpenEduAnalytics/tree/main/modules/Digital_Learning_Apps_and_Platforms/iReady) | For engagement/activity data pertaining to student lesson completion, and learning outcomes data in the context of student diagnostic assessment results. |


## Package Setup Instructions

To implement your own Digital Equity of Access Package, complete the following: 
- Install the most recent version of the OEA reference achitecture via the [OEA setup instructions](https://github.com/microsoft/OpenEduAnalytics#setup).
- Examine available data sources in Stage2p. See [above](https://github.com/microsoft/OpenEduAnalytics/tree/main/packages/Digital_Equity_of_Access#data-sources) for related data sources.
- Use a pipeline such the example [Package Pipeline](https://github.com/microsoft/OpenEduAnalytics/tree/main/packages/Digital_Equity_of_Access/pipelines) to combined data sources into a Power BI star schema model like the example provided in the [Data](https://github.com/microsoft/OpenEduAnalytics/tree/main/packages/Digital_Equity_of_Access/data) page. 
- Create a Power BI dashboard to explore Digital Equity of Access. Note the example [Package Pipeline](https://github.com/microsoft/OpenEduAnalytics/tree/main/packages/Digital_Equity_of_Access/pipelines) creates a SQL view which can be accessed via your Synapse workspace serveless SQL endpoint. Example dashboard concepts are [provided in this package](https://github.com/cviddenKwantum/OpenEduAnalytics/tree/main/packages/Digital_Equity_of_Access/powerbi).

## Package Components

This Digital Equity of Access package was developed by [Kwantum Analytics](https://www.kwantumanalytics.com/) in partnership with [Fresno Unified School District](https://www.fresnounified.org/) in Fresno, California. The architecture and reference implementation for all modules is built on [Azure Synapse Analytics](https://azure.microsoft.com/en-us/services/synapse-analytics/) - with [Azure Data Lake Storage](https://docs.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-introduction) as the storage backbone, and [Azure Active Directory](https://azure.microsoft.com/en-us/services/active-directory/) providing the role-based access control.

Assets in the Digital Equity of Access package include:

1. [Data](https://github.com/cviddenKwantum/oea-digital-learning-insights/tree/main/Digital_Equity_of_Access/data): For understanding the data relationships and standardized schema mappings used for certain groups of data.
2. [Documentation](https://github.com/cviddenKwantum/oea-digital-learning-insights/tree/main/Digital_Equity_of_Access/docs): [OEA Equity of Digital Access Package - Use Case Documentation](https://github.com/cviddenKwantum/oea-digital-learning-insights/blob/69dc247874cdec4aeac389a54d38d99d112e9a92/Digital_Equity_of_Access/docs/OEA%20Digital%20Learning%20Package%20-%20Access%20Use%20Case.pdf). 
3. [Notebooks](https://github.com/cviddenKwantum/oea-digital-learning-insights/tree/main/Digital_Equity_of_Access/notebooks): For cleaning, processing, and curating data within the data lake.
4. [Pipelines](https://github.com/cviddenKwantum/oea-digital-learning-insights/tree/main/Digital_Equity_of_Access/pipelines): For the overarching data processing (i.e., aggregation, subsetting, schema transformation, etc.), and support for PowerBI dashboards.
5. [PowerBI](https://github.com/cviddenKwantum/oea-digital-learning-insights/tree/main/Digital_Equity_of_Access/powerbi): For exploring, visualizing, and deriving insights from the data.

# Legal Notices
Microsoft and any contributors grant you a license to the Microsoft documentation and other content in this repository under the [Creative Commons Attribution 4.0 International Public License](https://creativecommons.org/licenses/by/4.0/legalcode), see the [LICENSE](https://github.com/microsoft/OpenEduAnalytics/blob/main/LICENSE) file, and grant you a license to any code in the repository under the [MIT License](https://opensource.org/licenses/MIT), see the [LICENSE-CODE](https://github.com/microsoft/OpenEduAnalytics/blob/main/LICENSE-CODE) file.

Microsoft, Windows, Microsoft Azure and/or other Microsoft products and services referenced in the documentation may be either trademarks or registered trademarks of Microsoft in the United States and/or other countries. The licenses for this project do not grant you rights to use any Microsoft names, logos, or trademarks. Microsoft's general trademark guidelines can be found at http://go.microsoft.com/fwlink/?LinkID=254653.

Privacy information can be found at https://privacy.microsoft.com/en-us/

Microsoft and any contributors reserve all other rights, whether under their respective copyrights, patents, or trademarks, whether by implication, estoppel or otherwise.

# WHAT IVY HAD ORIGINALLY
Student engagement in learning is the starting point for teaching and learning outcomes. Without engagement, learning is blocked. 

As teaching and learning increasingly use digital platforms and tools, and learning takes place outside of schools in digital learning environments, traditional attendance measures are not as representative of students’ actual engagement. Student attendance data is an important metric that schools track and derive insights from. Schools also need a way to measure students' digital activity across the different apps used for learning. With many schools’ transition to hybrid learning, having a way to combine students' in-person attendance in schools and their digital activity will be valuable for school systems. This combination provides a more comprehensive view of student engagement in learning than attendance data alone.

The Hybrid Engagement Package from OEA includes a set of assets for combining in-person attendance and digital activity, providing a more holistic representation of student engagement. This can be used by system and school leaders, and by teachers to identify:
 - Which schools and classes have higher and lower levels of hybrid engagement in learning, and whether expected patterns of engagement are continuing over time. 
 - Which schools and classes have higher and lower levels of in-person attendance or digital activities. This can be used to plan more precisely targeted programs or interventions to increase either attendance or use of digital learning tools, or both. 

The assets in this package can be combined with course completion, academic assessments, competency measures, mastery data, graduation rates, or other outcome data to identify how patterns of engagement relate to learning outcomes. With such combined data, schools and teachers can start to analyze whether new programs or interventions help to improve learning outcomes.  

![image](https://github.com/cviddenKwantum/OpenEduAnalytics/blob/3feaac196010f11d3cc925eb773b731cd3c37dea/packages/ContosoISD_hybrid_engagement/docs/images/PowerBI1.png)

This package was developed by Microsoft Education in partnership with Fresno Unified School District in California. The architecture and reference implementation for all assets is built on [Azure Synapse Analytics](https://azure.microsoft.com/en-us/services/synapse-analytics/) - with [Azure Data Lake Storage](https://docs.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-introduction) as the storage backbone,  and [Azure Active Directory](https://azure.microsoft.com/en-us/services/active-directory/) providing the role-based access control.

The assets currently represents data from Microsoft Teams for Digital Activities, but that source of data can be replaced with other types of digital activity data or combined with other sources of digital activity data if the school or system has access to those data. 

Assets in the hybrid student engagement package include: 

1. Documentation for ingesting data from multiple sources into the data lake.
2. Notebooks for cleaning, transforming, anonymizing and enriching data into the data warehouse.
3. PowerBI templates for exploring, visualizing and deriving insights from the data.

This package relies on 2 existing OEA modules:
1. [Contoso_SIS module](https://github.com/cviddenKwantum/OpenEduAnalytics/tree/main/modules/Contoso_SIS)
2. [M365 module](https://github.com/cviddenKwantum/OpenEduAnalytics/tree/main/modules/M365)

The hybrid student engagement package and its modules [welcome contributions.](https://github.com/microsoft/OpenEduAnalytics/blob/main/CONTRIBUTING.md) 

# Legal Notices

Microsoft and any contributors grant you a license to the Microsoft documentation and other content
in this repository under the [Creative Commons Attribution 4.0 International Public License](https://creativecommons.org/licenses/by/4.0/legalcode),
see the [LICENSE](LICENSE) file, and grant you a license to any code in the repository under the [MIT License](https://opensource.org/licenses/MIT), see the
[LICENSE-CODE](LICENSE-CODE) file.

Microsoft, Windows, Microsoft Azure and/or other Microsoft products and services referenced in the documentation
may be either trademarks or registered trademarks of Microsoft in the United States and/or other countries.
The licenses for this project do not grant you rights to use any Microsoft names, logos, or trademarks.
Microsoft's general trademark guidelines can be found at http://go.microsoft.com/fwlink/?LinkID=254653.

Privacy information can be found at https://privacy.microsoft.com/en-us/

Microsoft and any contributors reserve all other rights, whether under their respective copyrights, patents,
or trademarks, whether by implication, estoppel or otherwise.
