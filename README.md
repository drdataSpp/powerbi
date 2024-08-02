# Project 1: NZ Student Visa Approval Percentage and Total Decisions Analysis

## Project Description

This [project](https://github.com/drdataSpp/Spp_PowerBI_Student_Visa_Analysis/blob/main/Spp_PBI1_Student%20Visa%20Analysis.pdf) was built to serve the purpose of visualizing the NZ student visa approval percentage, rejection percentage, and total decisions took on the student visa applicants’ from India, Sri Lanka, Bangladesh, Nepal, and Bhutan from the year 2014 till May 2017. These country's visa applications are assessed by the *INZ Mumbai office*.

This analysis report gives insights on the countries approval % based on the year of application, the approval % based on the institute they applied for, the total decisions made by the INZ Mumbai Office every year and etc.

The second analysis report named [Student Visa Analysis By Indian States](https://github.com/drdataSpp/Spp_PowerBI_Student_Visa_Analysis/blob/main/Spp_PBI1.1_StudentVisa_IndianStates_Analysis.pdf) gives insights about the Indian states and their corresponding approval and rejection percentage based on the institutes (Private Education, Polytechnics and Universities) they applied for.


## How was the Analysis Report Done?

The raw data from the INZ website (https://www.immigration.govt.nz/assist-migrants-and-students/assist-students/international-markets/india) was in an unstructured manner. The excel file had the applicant's nationality and the year or the institute type as the row header, under this row header there were two sub-headers namely approval % and total decisions. Microsoft Power BI didn't accept this structure as a data source.

I created a new dataset based on the data from INZ where I created a new column for the year and institute type. By doing this, I ended up having only 4-row headers: Applicant Nationality, Approval %, Total Decisions, and Year or Institute type. Now the dataset was in a structured manner.

After doing this, I created a new column in Microsoft Power BI using the Power Query editor to find out the rejection % of all the countries in this dataset.

```
Rejection % = 1 - [#"Approval %"]
```

## Built with

[Microsoft Power BI](https://powerbi.microsoft.com/en-us/) - Business analytics service by Microsoft.

[Microsoft Excel](https://www.microsoft.com/en-us/microsoft-365/excel) - Spreadsheet developed by Microsoft.

## Credits & Acknowledgments

Thanks to the Immigration New Zealand for providing this data set.
