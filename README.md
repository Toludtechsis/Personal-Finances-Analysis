# Personal-Finance-Analysis
## A simple analysis on personal finances. 

![pexels-pixabay-164527](https://user-images.githubusercontent.com/17475689/195569714-8b7ea8eb-4d04-4e77-93d3-32e9798a502e.jpg) Image by Pixabay

## Project Background
The project features a simple case study on personal finances to derive insights into how money is being or earned spent over a period a of time.

- Project Objective
- Data Cleaning and Transformation
- Data Modeling
- Data Visualization and Analysis
- Insights
- Recommendations and Conclusions
- Visuals

## Project Objective

The objective of the project is to have a closer look into the finances of our case study, 
- To identify what expense is the highest ghrough the year
- To determine if expenses are within budget
- To determine if income is lower than expenses
- what expenses are the lowest
- What takes away the most money towards the end of the year
- What month has the most expense
- What month was budget exceeded
- Total expenses
- Total budget
- Total balance

## Data Cleaning and Transformation
The case study contained two dataset called Transaction and Budget. The dataset came in an xlsx file and the file was imported into Excel using the GetData tab within microsoft excel.
- After accessing the dataset and getting a quick view of the type of data I am working with, I inserted my dataset into a table.

<img width="555" alt="dataset" src="https://user-images.githubusercontent.com/17475689/195661277-3f71a012-a240-4287-95e1-83647b07418e.PNG">

- In order to clean the data I want to do the transformation in Power Query, so within the Data tool bar I clicked on get and transformed data to get into the Power query environment. 

<img width="834" alt="PowerQuery" src="https://user-images.githubusercontent.com/17475689/195662114-d49a82a9-04a0-43cd-8e23-25bf41a6c53b.PNG">

- After getting both my tables into PowerQuery, first step I take is to unpivot the date columns within the budget table. In order to have a row with a single record of information and have a corresonding structure with the rest of the dataset. 
- Promote first rows as headers.
- I created a dimensions table called categories that contains insights relevant to dimensions being described in transaction and budget tables
- I created another dimension table called Calender and purpose of this table having a uniform table take contains all the dates froom the earlies  date in the dataset to the latest date. I accomplished this writing Mcode using a blank query. 
- I confirmed that each cell has a single value, each column has the right data type.
- I also made sure each row represents a single record of information, then I closed and Loaded.


## Data Modeling
When I clicked on close and load, I choose the option to create as a connection and added to the data model. This loads all the 4 queries created into the data model.

<img width="438" alt="star schema" src="https://user-images.githubusercontent.com/17475689/195662457-72608adb-95eb-40b3-bc39-7e68d7391c37.PNG">

Using a star model schema I was able to connect the facts tables to dimensions table using primary and secondary keys, Then I proceeded to creating measures that would be needed for my analysis through the Power Pivot tab.

<img width="166" alt="My measures" src="https://user-images.githubusercontent.com/17475689/195665406-91b4cf2b-e0aa-415e-8e71-fe9406abd504.PNG">        <img width="311" alt="measures" src="https://user-images.githubusercontent.com/17475689/195666059-7a6c51ee-26c6-4274-802b-10b4a2816a0a.PNG">




## Data Analysis and Visualization
One of Microsoft Excel's famous tool is power pivot. 
Power Pivot allows us to summarize our data and be able to draw meaningful insights from the aggregations.
I used power pivot to derive insights on the objectives of the project. 
For our dimensions values such as actual, budget and balance I was able to use the pivot table to generate these values.

<img width="368" alt="measure pivot" src="https://user-images.githubusercontent.com/17475689/195707576-1067bf83-20ee-4330-a853-6702f427694e.PNG">


I was also able to use the power pivot tab to derive the sum of expenses and budgets on a monthly basis, which shows the picture of what budget was made for the month and what month expenses exceeded the budget or remained within budgets.

### Visualization

- Gender Distribution in Palmoria Group
Palmoria Group boast of a total of 946 employees, out of which 465 are Males, 441 Females and 40 without gender specification.

<img width="268" alt="company gender1" src="https://user-images.githubusercontent.com/17475689/194713236-0511e743-4fcb-4033-90c9-53b3408e8e59.PNG">

 
Gender distribution across Regions and Departments

The gender distribution across the 3 regions indicates a higher number of male employees. 
Kaduna with the most number of employees at 361 employees having 50.42% male employees, 45.71% female employees and 3.88% unspecified gender employees.
Abuja has 335 employees having 47.46% male employees, 47.16% female employees and 5.37% unspecified gender employees.
Lagos has 250 employees having 49.6% male employees, 47.2% female employees and 3.2% unspecified gender employees.

<img width="146" alt="regons gender" src="https://user-images.githubusercontent.com/17475689/194713327-0dd47031-b718-4e00-bd96-6fddad6981cb.PNG">  

Palmoria Group has 12 departments in operation and within the  departments, 7 departments have a high number of male employees and 5 deparments have more Female employees.


<img width="178" alt="gnde department1" src="https://user-images.githubusercontent.com/17475689/194713429-8dac4a4b-0079-4919-8a53-e46b8d769421.PNG">

- Gender distribution by employee ratings
In comparison to the other gender, there were more Females in the highest rated categories. The analysis revealed that more employees fall into the average group, which is dominated by men, as well as the two lowest rated categorie and 46% of the total 39 employees who are not classified by gender are rated average.

<img width="246" alt="emp rating" src="https://user-images.githubusercontent.com/17475689/194717495-00643ddb-a34a-4972-b230-5ca91f9578b5.PNG">


- Minimum Employee Payout Requirement
The analysis reveals that only 35% of the company's employees is paid the required minimum amount, which is $90000 for all manufacturing enterprises.

<img width="340" alt="min Pay" src="https://user-images.githubusercontent.com/17475689/194717759-138d34bf-e6f9-4a3e-8722-3907deb26175.PNG">


- Salary Pay Structure in Departments
Accounting, Human Resources, and marketing all showed glaring gender pay disparities, with Unspecified getting more money, while the Business Administration and Product Management departments were more evenly split between the genders across the board.

<img width="189" alt="gendar salary dep" src="https://user-images.githubusercontent.com/17475689/194717615-7b90f136-a42c-48b3-b0ac-93e33acb9bc9.PNG">

## Insights

-	Gender distribution gap across the organization has a relatively close, with Male employees only 3% more than the Females employees and 4% of the work force either gender neutral or unspecified.

-	Female employees have a generally higher performance rating compared to their Male counterparts.

-	Male employees across the company have an higher pay with an average salary earning of  $75k compared to the $72k of their Female counterparts and employees with unspecified gender having the highest salary average of $78k.

-	Male employees across all the three regions earn more than their Female counterparts with Kaduna having the widest pay gap within the organization.

-	7 departments of the 12 departments has more Male employees while 5 departments have more Female employees.

-	Palmoria Group does not meet the minimum employee pay requirement set for manufacturing companies and only has a 35% compliance rate.

-	A total of 26 employees earn between 0k - 20k, 103 employees earn up to 30k, 105 employees earn 40k, 96 employees earn 50k, 99 employees earn 60k, 117 employees earn 70k, 108 employees earn 80k, 90 employees earn 90k, 105 employees earn up to 100k and 97 employees earn up to 120k


## Recommendations and Conclusions

-	The Management should set up structures to even out gender distribution across regions. 

- Departments with wide difference in gender distribution should be investigated to ascertain the reason and steps taken towards a more balanced distribution in those departments.

-	The gap in gender pay should be addressed especially where 	qualifications and duties are the same.

-	High rating employees should be properly acknowledged for their hard works. "Happy employees, makes a thriving organization",

-	The Management should take necessary steps required to meet the minimum employee pay threshold.

## Visuals
- [Dashboard](https://github.com/Toludtechsis/OUI---Capstone---Project---Tolu/blob/5b1e3c04e533974c7d43d9fa8f64c193fb37e93f/Dashboard.PNG)
- [Report Page 1](https://github.com/Toludtechsis/OUI---Capstone---Project---Tolu/blob/bb95fec95a49ffb21c26a41e778e4537d72e2965/page1.PNG)
- [Report Page 2](https://github.com/Toludtechsis/OUI---Capstone---Project---Tolu/blob/493ee911c3a3b848339b6ff2bc52c27728bf0f50/page22.PNG)
