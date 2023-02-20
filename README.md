# Personal-Finance-Analysis
## A simple analysis on personal finances. 

![pexels-pixabay-164527](https://user-images.githubusercontent.com/17475689/195569714-8b7ea8eb-4d04-4e77-93d3-32e9798a502e.jpg) Image by Pixabay

## Project Background
The project features a simple case study on personal finances to derive insights into what an individual's finances looks like with emphasis on how money is being spent, what makes up the individual's expenses, how much income is being generated and through what channels over a period a of time.

- Project Objective
- Data Cleaning and Transformation
- Data Modeling
- Data Visualization and Analysis
- Insights
- Recommendations and Conclusions
- Visuals

## Project Objective

The objective of the project is to have a closer look into the finances of our case study, 
- To identify what expense is the highest through the year
- To determine if income is lower than expenses
- What month has the most expenses
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
Loading into the data model, I choose the option to create as a connection and added to the data model. This loads all the 4 queries created into the data model.

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

<img width="162" alt="rowsby budget" src="https://user-images.githubusercontent.com/17475689/195712115-6dba124e-341d-480f-8657-23ba84dbc6f6.PNG">


### Visualization
Visualization is almost my favorite part of data analysis. Getting to add visuals and show information I have been able to get from the data is interesting and empowering.

- Total Actual, Budget and Balance
The personal finance dataset has a total of 192,478 expenses, 230,502 budget, 38,024 balance. 
So it is evident that for the year expenses was not just within budget there was also more money left that could added to the following year.

<img width="300" alt="visual 1" src="https://user-images.githubusercontent.com/17475689/195715832-f8fe9ff9-c4b4-4f31-a8f0-3b2ef15c6461.PNG">

- Highest monthly expense. 
 The top 5 monthly expense include  social, medicals,charity, clothing, travel. The highest expense varies per month with each month telling a different story.
 
 <img width="281" alt="top 5 expenses" src="https://user-images.githubusercontent.com/17475689/195738244-75235a57-8f1f-422c-92de-ae6d772df9bd.PNG">
 
 - Determine if income is lower than expenses.
 Income appears to be generally higher than expenses, eventhough not by a significant margin. 
 There is the need for our case study to increase channels of income to ensure sustainability all year round.
 
 <img width="504" alt="Income" src="https://user-images.githubusercontent.com/17475689/195737263-d0e3651d-61e3-41c5-a246-849033f958aa.PNG">
 
 <img width="505" alt="expenses" src="https://user-images.githubusercontent.com/17475689/195737527-8ab26530-6cfd-44d6-ba8f-d6b5e1e8a3ae.PNG">
 
 
 - Determine if expenses are within budget.
 Expenses generally falls within budget except in months January and August.  
 
 <img width="341" alt="January" src="https://user-images.githubusercontent.com/17475689/195738048-2bcf7c83-eef1-47ba-b499-3b72601ca4f6.PNG">
 
 - What month has the most expenses.
 Janauary appears to be the month with the most expenses.
 
 <img width="667" alt="monthy actuals" src="https://user-images.githubusercontent.com/17475689/195738602-86b0402e-dcb5-47da-aa89-e835352a3f90.PNG">
 
 ### Sparklines and Slicers.
Slicers are often used as filters to give more precise insights into our data while sparklines describe the frequency of the degree of changes within a feature or metric.
I combined both sparklines and slicers in this analysis.
 
<img width="140" alt="sparkline" src="https://user-images.githubusercontent.com/17475689/195739174-ee7ea279-7607-457d-b58e-7260e9c58b50.PNG">

<img width="152" alt="slicers" src="https://user-images.githubusercontent.com/17475689/195739269-e32d3c9b-9118-49ce-8ac3-a0f90a45d6e5.PNG">

 
## Insights

-	It was deduced from the analysis that the case study is relatively a prudent spender who mostly stays within budget

-	Eventhough the case study tried not to exceed budget the margin between income and expense is too close which will not allow any form of buffer if expenses should go beyond budget. The case study could easily run into debt if unforseen expenditures present itself.

-	Anaysis showed that social activity is the number one expense incurred bythe case study, This might not be financially responsible way of life. 

-	Expenses are generally within budget but not exactly the case for January and August.  This could be due to January being the start of a new year and holiday cheer prompting decisions to spend more while the August spike could be due to summer time expenses. whatever the case maybe these months needs to be further investigated.


## Recommendations and Conclusions

-	The case study should identify more sustainable sources of income so as to increase the gap between expenses and income generated. 

- Months with beyond budget expenses should be investigated so as to determine the causesof the increased expense and better control incurring more expense.



## Visuals
[Dashboard](https://github.com/Toludtechsis/Personal-Finances-Analysis/blob/6e0a5166b5a618a2df253cfb3d0f193a96b7bcec/Dashboard.PNG)
