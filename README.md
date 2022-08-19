# Hybrid Student Engagement Package

The OEA Hybrid Student Engagement Package provides a set of assets which support an education system in developing their own holistic model to address and gauge hybrid student engagement. There are two main components of this package: 

1. <ins>Guidance and documentation:</ins> The [OEA Hybrid Student Engagement Package - Use Case Documentation]() provides guidance on the end-to-end process of developing a successful Hybrid Student Engagement use case project, including how to engage stakeholders in the project, prior research on the use case problem domain and theory, how to map data sources to the theory of the problem, and how to implement Microsoft’s Principles of Responsible Data and AI. <em> It is highly recommended this document be reviewed by any education system considering using this package, and that the documentation be revised to the specific data and decisions for that system’s context.  </em>
2. <ins>Technical assets:</ins> Various assets are freely available in this package to help accelerate implementation of Hybrid Student Engagement use cases. Assets include descriptions of data sources, notebooks for data processing, a pipeline for model building and deployment, and sample PowerBI dashboards. See descriptions of technical assets below.

<ins> Important Note:</ins> It is strongly recommended to education systems or institutions planning to use this package establish that they establish a process for obtaining student, family, guardian, teacher, faculty, and staff **consent for using this type of student engagement data**. This consent should be part of the system or institution’s **broader data governance policy** that clearly specifies who can have access to what data, under what conditions, for what purposes, and for what length of time.

This OEA Package was developed through a partnership between Microsoft Education, and [Kwantum Analytics](https://www.kwantumedu.com/).


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
