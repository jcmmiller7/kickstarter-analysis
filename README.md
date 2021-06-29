# kickstarter-analysis
Performing analysis on Kickstarter data to uncover trends

## Project Overview
The Kickstarter data set contains information on 4115 campaigns. Some of the important variables included in the data set include the outcome of the campaign (successful, failed, canceled, or live), the average donation to the campaign, the percentage funded (pledge to goal ratio), length of the campaign, and the category. The purpose of the project is to manipulate and analyze these variables to calculate statistical information in order to discover trends within the data. These trends are useful as they can be utilized by future kickstarters as a baseline to gauge potential success or failure prior to the campaign launch. Two deliverables were created to aid the user in their understanding of the data. The first is the outcomes based on launch date. The second is the outcomes based on goal. Graphical visualizations were created to bring the data to life. 

## Analysis and Challenges
The first part of the analysis involved filtering and sorting the data to make it more user friendly. A Years columns was added to the spreadsheet  using the year function in excel, which extracts the year from the date created conversion column. Next, a pivot table was created based on the parent category and years columns. Refer to the screenshot:

<img width="1364" alt="Screen Shot 2021-06-29 at 12 28 51 PM" src="https://user-images.githubusercontent.com/85506567/123834581-9129c700-d8d5-11eb-93b6-b06f0efd5aa4.png">

The pivot table was further manipulated to only include data based on theater outcomes and then a line chart was created to visualized this information. It is provided via screenshot:

![Screen Shot 2021-06-29 at 12 30 55 PM](https://user-images.githubusercontent.com/85506567/123834835-da7a1680-d8d5-11eb-93c1-686eb66e9b59.png)

The second part of the analysis involved using the count if function in excel to further visualize the percentage of successful, failed, and canceled plays based on the funding goal amount. A new spreadsheet was created for this data. Here is a screenshot of the new spreadsheet:

<img width="810" alt="Screen Shot 2021-06-29 at 12 34 17 PM" src="https://user-images.githubusercontent.com/85506567/123835253-54120480-d8d6-11eb-8b4d-aa4fd47b4775.png">

The columns in this spreadsheet were populated by altering the parameters of the count if function. For example, the 'number failed' column was populated by inserting these parameters into the count if function:
<img width="691" alt="Screen Shot 2021-06-29 at 12 37 24 PM" src="https://user-images.githubusercontent.com/85506567/123835610-c387f400-d8d6-11eb-8051-e5e20c0f7178.png">

Finally, a line chart was created to visualize the outcomes based on goals:

<img width="591" alt="Screen Shot 2021-06-29 at 12 42 31 PM" src="https://user-images.githubusercontent.com/85506567/123836244-7a846f80-d8d7-11eb-8c3b-af64b7efb7d1.png">


There were no challenges encountered during this project. However, some challenges the user may face include getting errors when trying to populate the percentage of the outcomes in the 'Outcomes Based on Goals Spreadsheet'. An error will arise if dividing by zero is trying to be calculated. This produces an undefined number and thus an error. The solution to this is to include the 'if error' argument the calculation, which will account for dividing by zero. Another challenge the user may face is working with the date columns in the kickstarter spreadsheet. The numbers that the column is initially populated with is based on unix timestamps. To make the dates more user-friendly, it is essential to convert to human readable dates. This can be done via the following:

<img width="1077" alt="Screen Shot 2021-06-29 at 12 52 18 PM" src="https://user-images.githubusercontent.com/85506567/123837443-d7ccf080-d8d8-11eb-947e-cc7750125ed7.png">


If this step is not completed, it will be difficult to work with the years column, which is essential in the analysis. 

## Results

One conclusion that can be made for the Theater Outcomes based on Launch Date deliverable is that the best month to launch a successful campaign is May. This month had 111 successful campaigns. This month also had the greatest ratio of successes to failures. The graph indicates that the early summer is overall the best time to launch a campaign due to the fact that May, June, and July had the greatest number of total successes. A second conclusion is that December is the worst time of year to launch a campaign. 46.6% of campaigns fail if launched during this month. One conclusion that can be made regarding the outcomes based on Goals spreadsheet is that 76% of the total campaigns with a fundraising goal of less than $1000 were successful. Most of the limitation for the data set are in regards to data integrity issues. Since this was created by a human entering data, there is likely some input errors which would skew the data. There were three duplicates. Another limitation is that many countries are considered and there measurements for certain columns are calculated using United States measurements. This will affect the accuracy of the data. Another limitation is the currency column because everything was analyzed via the US dollar. An additional table that could be made would filter the outcome by country. An additional graph that could be made could show average donation to number of backers ratio. This is interesting because we could draw conclusion on outcomes based on the number of backers and the amount of their average donation. Perhaps the most successful kick starters would have the greatest number of backers or if they depend on one very rich individual donation a large sum of money. It would be interesting to see how these factors influence outcome. 
