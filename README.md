# Attrition Rate of IBM Employees
### Reasons Why Employees leave the company

## Table of Contents

- [INTRODUCTION](#introduction)
- [PROJECT GOAL](#project-goal)
- [DATA SOURCE](#data-source)
- [TOOL USED](#tool-used)
- [EXPLORATION OF DATA](#exploration-of-data)
- [DATA PREPARATION](#data-preparation)
- [DATA ANALYSIS](#data-analysis)
- [FINDINGS](#findings)
- [RECOMMENDATIONS](#recommendations)



### INTRODUCTION
IBM, or International Business Machines Corporation, also known as “Blue Sky” is a global technology and consulting company founded in 1911. It is known for its diverse portfolio of products and services, ranging from hardware like mainframes and servers to software solutions and cloud computing services. However, the company has faced challenges regarding employee turnover. Despite its long history of innovation in computing and information technology, the company has experienced significant fluctuations in its workforce. 
Attrition rate,  a voluntary and involuntary departures of employees from an organization, carries substantial implications for IBM's workforce management, productivity, and overall business performance. Elevated attrition rates within IBM could lead to increased recruitment and training expenditures, the erosion of institutional knowledge and expertise, diminished employee morale and engagement, and potential disruptions to project timelines and deliverables. Addressing and mitigating high attrition rates is critical for IBM to sustain a stable and productive workforce, ensuring continued success and competitiveness in the market.
This analysis explores the multifaceted landscape of employees attrition within IBM, seeking to unveil nuanced insights into the root causes, patterns, and trends driving employee turnover. By comprehending these dynamics, IBM can pinpoint areas of vulnerability, deploy tailored retention tactics, and tackle the fundamental drivers of attrition head-on.

![HR Attrition Rate Updated - Excel Dashboard](https://github.com/Olabisy/IBM-HR-Employees-Attrition-Rate/assets/114803890/c63bc6f3-fc20-488c-aa95-10d183d1741c)


### PROJECT GOAL
The central aim of this analysis is to uncover the core reasons driving employee departures from IBM and to identify specific areas within the company where turnover rates are particularly high. By understanding the underlying motivations behind employee exits and pinpointing the departments experiencing elevated turnover, IBM can develop targeted strategies to address these issues and improve overall retention efforts.

### Tool used
- Microsoft Excel 


### DATA SOURCE
The primary data used for this project is downloaded from Kaggle.com, containing detailed information about each employee

### EXPLORATION OF DATA
The dataset comprises 1,470 rows representing individual employees at IBM, with 35 columns representing various attributes such as age, marital status, business travel frequency, distance from home, and education level, among others. The dataset was sourced from Kaggle in the form of an MS Excel spreadsheet.
Prior to analysis, the dataset underwent thorough checks for duplicate entries and missing values. Fortunately, no duplicates were found, and there were no missing values requiring attention. 
Certain categorical attributes or columns in the dataset were encoded numerically using values ranging from 1 to 5. These numerical representations will be adjusted to their respective categorical attributes during the later stages of analysis
The data was then exported to Power Query within MS Excel for cleaning and transformation processes to ensure its readiness for subsequent analysis.


### DATA PREPARATION
 After exporting the data into Power Query, I meticulously reviewed the data types of each attribute and adjusted where necessary to ensure consistency and accuracy. Utilizing the "Add Column" function in the Power Query ribbon, I created new columns to enhance the dataset.
For instance, the "Education" column, which was originally coded with values ranging from 1 to 5, was replaced with a new column representing the actual education levels. Here's the transformation:
- Created a new column for education.
-  Replaced the numerical values with their corresponding education levels:
    - 1 = Bellow College
    - 2 = College
    - 3 = Bachelor
    - 4 = Master
    - 5 = Doctor
   
- Changed the data type of the newly added column to "Text" to accurately reflect the categorical nature of the education levels.
  
Similarly, other columns such as "Job Satisfaction" underwent a similar transformation. By creating a new column and replacing the numeric values with their corresponding attribute descriptions, the dataset was enriched for clarity and analysis. For instance:
  - 1 = Low
  - 2 = Medium
  - 3 = High
  - 4 = Very High
    
I applied the same steps for Environment satisfaction, Job Involvement, performance rating etc.

In addition, I 
- created a new "Age Bucket" column: This groups age ranges into categories ("18-25", "26-35", etc.) to understand which age groups are more impacted by attrition.
- grouped Monthly Income: Categorizing income as "Low", "Average", and "High" allows for broader analysis of income's role in employee churn.
- grouped Distance from Home: Categorizing distances as "Nearby", "Far", and "Very Far" simplifies analysis and highlights potential location-related factors in employee turnover.
Numbers of years worked was also grouped into “btw 0-10“, “btw 11-20“, “21-30” and “over 31.”

Also, some unnecessary columns were removed such as “Over 18” column which contains redundant value that is the column contains the same value.

### DATA ANALYSIS
In this analysis, a total of 1,470 employees were included, out of which 1,233 employees are currently employed at the company, while 237 employees have experienced attrition. This attrition represents approximately 16% of the total workforce.

1. **Attrition by Gender**

    Taking gender into account, approximately 60% of the employees, totaling 882 individuals, were male. Among them, around 10.2% (150 employees) have experienced attrition.
    Female employees accounted for 40% of the workforce, with a total of 588 individuals. Within this group, approximately 5.9% (35 employees) are now ex-employees.
   
  ![Gender](https://github.com/Olabisy/IBM-HR-Employees-Attrition-Rate/assets/114803890/b5abb9c6-f161-4645-bf1c-cf08d67ded7e)

    
2. **Attrition by Marital Status**

   Out of the total 1,470 employees, approximately 45.8% were married, 31.9% were single, and 22.2% were divorced. Interestingly, based on the data, it appears that single employees have the highest attrition rate, followed by married employees. This suggests that marital status may play a role in employee turnover within the company. Further analysis could delve into the reasons behind this trend and explore potential strategies to improve retention among single and married employees.

   ![Marital status](https://github.com/Olabisy/IBM-HR-Employees-Attrition-Rate/assets/114803890/175fb7dd-3475-4f7e-8434-eef2f01a987e)


3. **Attrition by Age**

     The data indicates that employees between the ages of 25-35 tend to leave the company more frequently compared to older age groups. One possible explanation for this trend could be the eagerness of younger employees to explore career advancement opportunities. 
Younger individuals often have a strong desire for career growth and may be more inclined to seek new challenges and opportunities outside of their current organization. This eagerness for career advancement could contribute to higher turnover rates among younger employees.
Additionally, younger employees may be more willing to take risks and pursue new opportunities that align with their career goals, leading them to leave their current company more easily. This propensity for career change and advancement among younger individuals may contribute to the observed higher attrition rates in this age group.

    ![Age](https://github.com/Olabisy/IBM-HR-Employees-Attrition-Rate/assets/114803890/22ee9378-293b-4185-829e-b5d7f7e02453)

4. **Attrition by Business Travel**

   The data shows that employees who rarely travel on business trips tend to leave the company at a faster rate compared to those who frequently travel. The reason for this could be employees who rarely travel may feel stagnant in their roles and opportunities for growth. Lack of exposure to different environments and experiences may lead to disengagement and ultimately attrition.
 
    ![Business Travel](https://github.com/Olabisy/IBM-HR-Employees-Attrition-Rate/assets/114803890/791bc86c-67e4-48f1-841d-4791fedbb064)


5. **Attrition by Department**

    The data shows that employees who rarely travel on business trips tend to leave the company at a faster rate compared to those who frequently travel. The reason for this could be employees who rarely travel may feel stagnant in their roles and opportunities for growth. Lack of exposure to different environments and experiences may lead to disengagement and ultimately attrition.

    ![Department](https://github.com/Olabisy/IBM-HR-Employees-Attrition-Rate/assets/114803890/fdf2d449-1315-49f5-8c3c-b03e67f6c0b3)

  
6. **Attrition by Monthly Income**
   
     It's reasonable to say that income is a significant factor contributing to attrition rates, particularly in the Research and Development (R&D) and Sales departments, based on the provided data.
In the R&D department, where approximately 47.8% of employees earn a low monthly salary, it's plausible that compensation plays a role in attrition. Employees in R&D roles often possess specialized skills and qualifications, and they may seek higher-paying opportunities elsewhere if they feel their contributions are not adequately recognized or compensated.
Similarly, in the Sales department, where about 19.5% of employees earn a very low income, it is notable that the attrition rate is also high. Sales roles are often performance-driven, and employees may feel demotivated if they perceive their compensation to be insufficient relative to their efforts and results.
 
   ![Income](https://github.com/Olabisy/IBM-HR-Employees-Attrition-Rate/assets/114803890/add6787b-a796-4d1f-afdd-cf7a517b9fc5)


7. **Attrition by Job Roles**

    Sales Executives, Research Scientists, and Laboratory Technicians are the job roles experiencing the highest attrition rates within the company. Further analysis reveals that these roles also have lower incomes compared to others within the organization. On the other hand, roles such as Research Directors and Managers typically command higher pay.
The correlation between lower income levels and higher attrition rates among Sales Executives, Research Scientists, and Laboratory Technicians suggests that compensation may indeed be a significant factor influencing attrition in these roles. Employees in these positions may feel undervalued or financially constrained, leading them to seek opportunities elsewhere where they can receive higher compensation for their skills and contributions.

   ![Job Roles](https://github.com/Olabisy/IBM-HR-Employees-Attrition-Rate/assets/114803890/6b7b1270-0a5d-40ee-95f7-a1e076c184af)


8. **Attrition by Education**

    Employees with Bachelor's and Master's degrees exhibit higher attrition rates within the company, despite earning the most in the organization. I delve in deeper to see if there is any factor triggering their churn, surprisingly, job satisfaction levels among these degree holders reveals there is a considerable level of satisfaction. Their monthly income is also examined, they are the highest paying employees in the company.
Dissatisfaction with salary or job satisfaction is not the primary reasons for their departure. Instead, it's likely that the decision to leave is driven by a desire for career advancement and exploration.

  ![Education](https://github.com/Olabisy/IBM-HR-Employees-Attrition-Rate/assets/114803890/8ca63440-8593-496a-a5bb-b56b5f0b1214)


9. **Attrition by Distance from Home**

   Based on the visualization, it appears that distance from home may not have a significant impact on the attrition rate within the company. Majority of employees seem to live relatively close to their workplace, suggesting that commuting distance may not be a major factor influencing their decision to leave the company.

    ![Distance from home](https://github.com/Olabisy/IBM-HR-Employees-Attrition-Rate/assets/114803890/88efd049-771e-4dff-bcdf-b9960d853b1b)


10. **Attrition by Work Experience**

    Based on the dataset, employees who have spent fewer than 10 years in a company tend to have a higher tendency to leave.

    ![Total working yrs](https://github.com/Olabisy/IBM-HR-Employees-Attrition-Rate/assets/114803890/c2f0ab57-3c9a-435e-bac0-d10ea9f288e1)


11. **Attrition by Number of Companies Worked**

    Employees who have only worked for one company may have a higher likelihood of leaving, driven by a desire to explore opportunities outside of their current organization. Often referred to as "job hopping”.
    ![Number of company worked](https://github.com/Olabisy/IBM-HR-Employees-Attrition-Rate/assets/114803890/7a36474f-6ec1-4123-a71f-8a5d841c7198)


12. **Attrition by Training Times**

     It's intriguing to note that the number of training sessions attended in the previous year does not appear to have a significant impact on the attrition rate. In fact, employees who attended training two or three times in the previous year seem to have higher attrition rates.
  
  ![TrainingTimes](https://github.com/Olabisy/IBM-HR-Employees-Attrition-Rate/assets/114803890/7cafbc1b-8f2f-4e5b-8ba1-889b09afebd0)


### FINDINGS
- Male gender appears to have higher attrition compared to female employees within the company.
- Married employees exhibit a higher tendency to change jobs more than single employees, while divorced employees show little inclination to leave their positions.
- Employees aged between 25 and 35 are more likely to leave the company.
- Those who rarely travel for business purposes are more susceptible to attrition.
- The Research and Development department experiences the highest attrition rate among all departments.
- Monthly income emerges as a critical factor influencing employee departures.
- Sales Executives, Research Scientists, and Laboratory Technicians are the top three job roles with the highest  attrition rates.
- Education and work-life balance do not significantly impact the attrition rate, as a considerable percentage of employees’ report maintain a good work-life balance.
- Employees who have only worked for one company exhibit a higher likelihood of leaving, possibly driven by a desire for exploration or career advancement.
- Employees with less than 10 years of tenure at the company are more prone to leaving their positions.


### RECOMMENDATIONS
- IBM should review the salary structures for departments experiencing the highest attrition rates. Adjusting salaries to remain competitive within the industry can help retain top talent and reduce turnover.
- Encourage Business Travel and improve travel packages. IBM should review and potentially enhance travel packages to better support employee engagement and retention.
- IBM should reevaluate its compensation structures to ensure that employees in roles with high attrition rates are fairly rewarded for their work.
- Conducting exit interviews, surveys, or focus groups with departing employees can provide valuable insights into the reasons for attrition and identify areas for improvement within departments. IBM should use this feedback to inform retention strategies and initiatives.















