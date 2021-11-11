
# HR- SELECTION-ANALYSIS-

•	Objective: In this problem is employees are lefting the company and company wants to stop them, so they want which employee has higher chances to mostly focus on them.  

•	In this we used various factors such as : satisfaction_level, number_project, promotion_last_5years, Department, salary, etc. and analyzed it


## Install dependecies
numpy 
```
!pip install numpy 
```
pandas
```
!pip install pandas
```
matplotlib
```
pip install matplotlib
```

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

![Screenshot (380)](https://user-images.githubusercontent.com/62400307/141348852-d747a8d1-c83d-4451-a2f8-baa529e9540b.png)


## Data exploration and visualization

Average numbers for all columns

![Screenshot (381)](https://user-images.githubusercontent.com/62400307/141348906-413cb274-60e1-4972-a439-b0945497a008.png)


From above table we can draw following conclusions,

    1. Satisfaction Level**: Satisfaction level seems to be relatively low (0.44) in employees leaving the firm vs the retained ones (0.66)
    2. Average Monthly Hours**: Average monthly hours are higher in employees leaving the firm (199 vs 207)
    3. Promotion Last 5 Years**: Employees who are given promotion are likely to be retained at firm


Impact of salary on employee retention


![Screenshot (382)](https://user-images.githubusercontent.com/62400307/141348988-0f7c06ef-6904-4717-9937-da4b59df0d55.png)


Above bar chart shows employees with high salaries are likely to not leave the company



Department wise employee retention rate

![Screenshot (383)](https://user-images.githubusercontent.com/62400307/141349037-6a7339dc-d82f-4cd7-b2fd-9e78b0202a08.png)



From above chart there seem to be some impact of department on employee retention but it is not major hence we will ignore department in our analysis

From the data analysis so far we can conclude that we will use following variables as independant variables in our model

    1. Satisfaction Level**
    2. Average Monthly Hours**
    3. Promotion Last 5 Years**
    4. Salary**



Tackle salary dummy variable

Salary has all text data. It needs to be converted to numbers and we will use dummy variable for that. Check my one hot encoding tutorial to understand purpose behind dummy variables.



And in the end applied **Logistic Regression** and get an **accuracy** of **78.42%**, which help company, to mostly focus on employee which has higher chances to left the company.  

