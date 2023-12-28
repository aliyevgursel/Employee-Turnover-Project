# Employee-Turnover-Project

**Project Title**

Employee Turnover Project: Providing Data-Driven Suggestion to HR



**Project Overview**

This capstone project was part of Google Advanced Data Analytics Professional Certificate program. It provided an opportunity to analyze a dataset and build predictive models that can provide insights to the Human Resources (HR) department of a large consulting firm.

This hypothetical firm, Salifort Motors, had a high rate of turnover among its employees. The task was to design a model that predicts whether an employee will leave the company based on their job title, department, number of projects, average monthly hours, and any other relevant data points. The analysis and the model indicated that the high employee turnover is mostly due to overwork.

Two ML models were built: Extreme Gradient Boosting (XGB) and Random Forest (RF) models. Both models predicted the turnover status fairly well. The best among those was XGB model. It had the following evaluation metric test scores: recall = 0.93%, f1 = 94%, precision = 95%, accuracy = 98%. Top five predictive features of the employees' turnover are 1) job satisfaction, 2) average monthly work hours, 3) last evaluation scores, 4) number of projects and 5) tenure. The independent variables with the lowest feature importance were salary levels, promotion in the last 5 years and department.



**Business Understanding**

About 17% of the employees left the company. The HR department and the leadership needed a good predictive model that would help the company increase retention and job satisfaction for current employees, and save money and time training new employees. 



**Data Understanding**

This was a hypothetical survey dataset collected by the HR department. The dataset had about 15k observations with 10 different variables like employee satisfaction, average monthly work hours, last employee evalution score, salary, department etc. The initial descriptive analysis showed that the "optimal" average monthly work hours would be within 168 -210 hours. At this range the turnover rate is minimal.

![image](https://github.com/aliyevgursel/Employee-Turnover-Project/assets/68837397/1474bccf-c20a-4f6d-a7d4-30a8a3590de0)

The dataset had some duplicate entries, which were droped before the analysis. Also, some categorical variables were reformatted into binary variables.



**Modeling and Evaluation**

The XGB model was used as the main predictive model since it had the highest evaluation metric test scores: recall = 0.93%, f1 = 94%, precision = 95%, accuracy = 98%. Below is the confusion matrix for the model:
![image](https://github.com/aliyevgursel/Employee-Turnover-Project/assets/68837397/7614be1f-5128-4110-953c-1864df02a17f)


This model was also used to identify the main predictive features of the employees' turnover.
![image](https://github.com/aliyevgursel/Employee-Turnover-Project/assets/68837397/52a216e8-0a71-4d25-8e27-3a568d5fed8d)



**Conclusion**

The analysis showed that those who left the company were most likely to be overworked or underworked, had lower job satisfaction, and contributed to more projects.
Interestingly, those who left also had slightly higher last evaluation scores. The median last evaluation score was 0.79 for them, whereas for those who stayed it was 0.71.

While there was some variation in the turnover rate between the department, employees' department had lowest feature importance in the model. This may mean that factors affecting the turnover are more or less the same across the departments. Among the department variables RandD had the highest feature importance. This may not be surprising since it has one of the lowest turnover rates.

The key recommendations based on the analysis were following:
- Make sure that the employees work 'optimal' hours (168-210 hours per month).
- Keep track of employees who have high evaluation scores but low job satisfaction. Figure out why these employees have low satisfaction levels. Can they be promoted and/or have a raise? Also make sure that these employees have at least medium level of salaries.
- Figure out what factors help the RandD department to have the lowest turnover rates, and see if it is possible to apply these factors to the other departments.
