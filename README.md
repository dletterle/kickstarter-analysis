# An Analysis of Kickstarter Campaigns
Performing analysis on Kickstarter data to uncover trends

**#Deliverable 1**

The excel file was downloaded and modules were followed 
The excel file name was changed from StarterBook.xlsx to Kickstarter_Challenge.xlsx
A separate folder was created to hold the charts that were created 
A "Years" column was created utilizing the Year() function from the "Date Created Conversion" and Date was coverted utilizing Epoch Time Converter
A Pivot Table was created and placed in a separate sheet titled "Outcomes Based on Launch Date" 
	Pivot Table was filtered by "Parent Category" and "Years" 
	"Outcomes" were placed in Columns 
	"Date Created Conversion" was placed in Rows
	"Count of outcomes" was placed in Values 
	The "Parent Category" filter was filtered to "theater"
The line chart seen below was created	
	![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/99268646/154607482-c6237c13-b4de-4885-84c4-6dd420199e3c.png)

**#Deliverable 2**

A new sheet "Outcomes Based on Goals" was created within Kickstarter_Challenge.xlsx
The following columns were created: Goal, Number of Successful, Number Failed, Number Canceled, Total Projects, Percentage Failed, Percentage Canceled 
The "Goal" column was created with dollar-range amounts 
The table was populated through "COUNTIFS()"
The data was checked through the "SUM()" function of the created table with "COUNTIFS(>=0)"
The "SUM()" function was used to populate the "Total Projects" column with the number of successful, failed, and canceled projects for each row 
The percentage of successful, failed and canceled projects for each row by dividing each cell by the total summed and changing the format of the cell to "percentage"
A line chart was created to visualize the relationship between the goal-amount and the percentage of successful, failed, or canceled projects. 

<img width="569" alt="Outcomes_vs_Goals" src="https://user-images.githubusercontent.com/99268646/154712183-8de17ef5-0707-4a84-bda2-827b878d7511.png">

**Deliverable 3**

_Section 1 Overview of Project_

The purpose of this analysis was to help Louise with her project campaign. This was done by becomming familiar with Excel and some of the basic functions and formatting to review the data collected by Louise and turn it into a more user-friendly readable format. Some of the features utilized in this project to assist Louise include: filtering, formatting and freezing; conditional formatting; finding averages, quartile values, minimum annd maximum values, and variance and standard deviation; errors and debugging; pivot tables; charts and diagrams. 

_Section 2 Analysis and Challenges_

	_Analysis_

When performing analysis of the data collected by Louise the data was downloaded and properly saved in Excel. Then the rows,columns, sheet names and data type were appropriately noted. A pane was created with the first three columns and title row. Conditional rules were created to show "successful" outcomes in green; "failed" outcomes in red; "live" outcomes in blue; and "canceled" outcomes in yellow. Next Error donations were changed to "0" due to the fact that numbers cannot be divided by zero. Pivot tables were created for categories and subcategories with the graphs: 

![image](https://user-images.githubusercontent.com/99268646/153982455-eab881ea-7c55-4694-9c2f-5fb61fbc5632.png)
![image](https://user-images.githubusercontent.com/99268646/153982492-13461871-4b6d-4095-9de8-984bf8591c2a.png)

When searching the play _Walken on Sunshine_ the status was **successful** the average donation was **$71.24** rhe duration was **30 days** and the number of backers was **173 **hfhf**fjfjf
VLOOKUP was used to depict the following averages for donations and backers
![image](https://user-images.githubusercontent.com/99268646/153983211-152385b6-6a02-49bc-8eea-f1c637633cb8.png)
Mean and median goal and pledge amounts were found for "successful" and "failed" "US" "plays" 
Mean and median goal and pledge amounts were found for "successful" and "failed" "US" "pop music"; and "US" "wearable tech"
Standard deviation, upper quartile, lower quartile, and range were found for both "successful" and "failed" "goal" and "pledged" amounts
Kickstarter	Successful	Failed			Music/ pop	Successful	Failed			Wearable Tech	Successful	Failed
Mean Goal	$5,049	$10,554			Mean Goal	$4,017	$40,400			Mean Goal	$18,040	$50,064
Median Goal	$3,000	$5,000			Median Goal	$2,500	$11,000			Median Goal	$12,000	$27,500
Standard Deviation of Goal	$7,749	$21,968										
Upper Quartile of Goal	$5,000	$10,000										
Lower Quartile of Goal	$1,500	$2,000										
IQR of Goal	$3,500	$8,000										
												
Mean Pledged	$5,602	$559			Mean Pledged	$4,758	$229			Mean Pledged	$26,243	$7,639
Median Pledged	$3,168	$103			Median Pledged	$3,460	$26			Median Pledged	$18,855	$837
Standard Deviation of Pledged	$8,335	$1,331										
Upper Quartile of Pledged	$5,699	$501										
Lower Quartile of Pledged	$1,717	$9										
IQR of Pledged	$3,982	$492										
![image](https://user-images.githubusercontent.com/99268646/153984075-f96c8172-f75b-455d-953b-e6fde4146d54.png)
Outliers were found and Box-charts were created 
![image](https://user-images.githubusercontent.com/99268646/153984402-b98ac746-5e03-47fa-a13d-d962b15dc5a3.png)
	
	_Challenges__
My largest challenge was using the conditional statements to filter the data. At first I struggled attempting to do the obvious and just remove the excesss data through deleting or hiding the cells leaving the remaining cells for analysis. After further research and evaluation it was apparent that the dataset needed to be filtered using conditional formatting. I went back to the module to review conditional formatting and fixed my analysis and workbook. 

_Section 3 Results_
	
	_Conclusions about the Theater Outcomes by Launch Date_
When reviewing the Theater Outcomes by Launch Date, there is a much higher count of successful theater outcomes done in the summer months (May, June, July) with the largest count of successful theater outcomes in May. Failed outcomes for theater concerts seem to remain relativeley consistent through the year with failed outcomes creating a much flatter line compared to the line generated from successful outcomes. It appears the worst month to have a theater concert is December where there is almost a 1:1 ratio of failed to successful outcomes of theater concerts. 
	
	_Conclusion Outcomes Based on Goals_
When reviewing the Outcomes Based on Goals there is no relationship between the variables "Goal" and "Outcome"; as in, these variables are independent from one another. As goal amount increases or decreases, there is no impact on the percentage of success or percentage of failure of plays. It is also easy to see the independence of the variables when looking at the graph because there is no relation and an ever changing slope. On a practical experience this makes sense because a goal is not necessarily action. So a goal of an A in a course or a budget of 50,000 does not determine outcome like other variables such as "study time" or "pledged amount" 

	_Limitations_
There are a few limitations of the dataset. There are some extreme outliers in the dataset. In just viewing the box plot of "Great Britain Thearter Market Goals and Pledged" there are two outliers, one for "goals" and one for "pledged" that increase the mean and standard deviation. Also some of the subcategories are too small to generate meaningful analysis. Which also impacts outcome variables because for some subcategories such as Pop/Music only has 39 values and they are all successful which limits reliability and analysis of specific categories. It is also a limitation to make a recommendation based on any category related to "goal". As described previously I have the goal of an A as the plays have a monetary goal that we are not aware of how it is generated. The goal could just be a guess and hope. Without the time spent on the module or the money actually generated, the goal does not offer much statistical analysis. 

	_Other tables and/or graphs_
Some other tables that would be meaninful to see if there is a way to predict success, specifically in the US, and then increase to other countries if the calculations hold true. As we see in the data, Theater is more likely to have a successful outcome in May, but why? Is it due to just time of the year, or is there further analysis that can be done. To do this Louise would start by running pivot tables of data with US as the filter and strictly doing all categories as the row and outcome as the column. Next tabulate all categories successful and failed outcomes. Run averages and percentages to review the categories with the highest percentage of success and the highest percentage of failure. Maybe select the five highest percentages in each category. After this is done drill down further with pivot tables to see if there is a relationship between the percentages. For example is all "Music"the most failed category because it requires the largest goals or and has the shortest gap in date created and date ended or is it only one subcategory within Music in the US that increases the number of failed outcomes. Perhaps the subvategory Rock and Pop actually have a high rate of successful outcomes and Jazz has a high rate of failed outcomes. Then further pivot tables can be done to review even more variables (i.e. the time of year the event occured and the count of backers). After quite a lengthy bit of analysis (and a few t-tests for significance) Louise would have the ability to increase the prediction of successful outcomes. 
