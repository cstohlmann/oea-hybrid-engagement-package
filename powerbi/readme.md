# Power BI Dashboards

The OEA Hybrid Engagement Package Power BI template enables users to quickly explore data. There are two options for exploring this module Power BI template.
- [Power BI with test data](https://github.com/cstohlmann/oea-hybrid-engagement-package/blob/main/powerbi/Hybrid%20Engagement%20Package%20Dashboard%20TestData.pbix): Power BI templated with module test data imported locally. 
- [Power BI with direct query](https://github.com/cstohlmann/oea-hybrid-engagement-package/blob/main/powerbi/Hybrid%20Engagement%20Package%20Dashboard%20DirectQuery.pbix): Power BI template connected to a Synapse workspace data source. See instructions below to setup.

See [Power BI setup instructions](https://github.com/cstohlmann/oea-hybrid-engagement-package/tree/main/powerbi#power-bi-setup-instructions) below for details.

## Dashboard Explanation 

The OEA Hybrid Engagement Package Power BI template consists of a single dashboard which summarizes the status of hybrid engagement at a distict-level. 

Use the tool-tips provided on the visuals to understand the purpose of each data visualization.

## Overview of Hybrid Engagement

| ![Overview of Hybrid Engagement](https://github.com/cstohlmann/oea-hybrid-engagement-package/blob/main/docs/images/pbi_p1_overview_of_hybrid_engagement.png "Overview of Hybrid Engagement") |
|:--:|
| <b> Summary of the status of hybrid engagement in the district by school and student grade-level. </b>|

## Power BI Setup Instructions

<strong><em>IMPORTANT NOTE:</strong></em> To replicate the example template with test data (provided), as mentioned before - you will need to execute the Digital Engagement Schema Pipeline, each of the module pipelines, and this package pipeline. You will then pull the tables from 3 different databases: 
 - sqls2_contoso_sis: studentattendance_pseudo table,
 - sqls2_digital_activity: digital_activity table, and
 - sqls3_hybrid_engagement: Student_pseudo table.

#### [Power BI with imported test data](https://github.com/cstohlmann/oea-hybrid-engagement-package/blob/main/powerbi/Hybrid%20Engagement%20Package%20Dashboard%20TestData.pbix):
1. Download the PBIX file with test data here: [LINK](https://github.com/cstohlmann/oea-hybrid-engagement-package/blob/main/powerbi/Hybrid%20Engagement%20Package%20Dashboard%20TestData.pbix)
2. Open the link locally on your computer and explore module test data. 
3. Connect to the Digital Engagement SQL db: sqls2_digital_activity, and pull in the digital_activity table. This table is the only one that requires a DirectQuery.

#### [Power BI with direct query of data on your data lake](https://github.com/cstohlmann/oea-hybrid-engagement-package/blob/main/powerbi/Hybrid%20Engagement%20Package%20Dashboard%20DirectQuery.pbix):
- Complete the [module setup instructions](https://github.com/cstohlmann/oea-hybrid-engagement-package#package-setup-instructions).
- Download the PBIX file with direct query here: [LINK](https://github.com/cstohlmann/oea-hybrid-engagement-package/blob/main/powerbi/Hybrid%20Engagement%20Package%20Dashboard%20DirectQuery.pbix)
- The dashboard visuals may not load. You will need to switch your Synapse workspace serverless SQL endpoint by:
    - Select menu item File > Options and settings > Data source settings.
<kbd> 
    <img src="https://github.com/microsoft/OpenEduAnalytics/blob/main/modules/module_catalog/Clever/docs/images/pbi%20data%20source.png" width="600"> 
</kbd>

    - Select Change Source...
| <img src="https://github.com/microsoft/OpenEduAnalytics/blob/main/modules/module_catalog/Clever/docs/images/pbi%20change%20source.png" width="600"> | 
|-|
    - Enter your Synapse workspace SQL server endpoint. This can be found on your Synapse workspace information page in the Azure portal.
<kbd> 
    <img src="https://github.com/microsoft/OpenEduAnalytics/blob/main/modules/module_catalog/Clever/docs/images/pbi%20sql%20endpt.png" width="600">
</kbd>
<kbd> 
    <img src="https://github.com/microsoft/OpenEduAnalytics/blob/main/modules/module_catalog/Clever/docs/images/synapse%20sql%20enpt.png" width="600"> 
</kbd>
