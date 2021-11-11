
# HR- SELECTION-ANALYSIS-

•	Objective: In this problem is employees are lefting the company and company wants to stop them, so they want which employee has higher chances to mostly focus on them.  

•	In this we used various factors such as : satisfaction_level, number_project, promotion_last_5years, Department, salary, etc. and analyzed it

## DATA
| Features |
| :-------- |
| satisfaction_level|
| last_evaluation|
| number_project|
| average_montly_hours |
|  	time_spend_company |
| Work_accident |
| promotion_last_5years |
| Department |
| left|


## Data exploration and visualization

Average numbers for all columns


From above table we can draw following conclusions,

    1. Satisfaction Level**: Satisfaction level seems to be relatively low (0.44) in employees leaving the firm vs the retained ones (0.66)
    2. Average Monthly Hours**: Average monthly hours are higher in employees leaving the firm (199 vs 207)
    3. Promotion Last 5 Years**: Employees who are given promotion are likely to be retained at firm


Impact of salary on employee retention



Above bar chart shows employees with high salaries are likely to not leave the company



Department wise employee retention rate




From above chart there seem to be some impact of department on employee retention but it is not major hence we will ignore department in our analysis

From the data analysis so far we can conclude that we will use following variables as independant variables in our model

    1. Satisfaction Level**
    2. Average Monthly Hours**
    3. Promotion Last 5 Years**
    4. Salary**



Tackle salary dummy variable

Salary has all text data. It needs to be converted to numbers and we will use dummy variable for that. Check my one hot encoding tutorial to understand purpose behind dummy variables.



And in the end applied Logistic Regression with an accuracy of 78.42%,
