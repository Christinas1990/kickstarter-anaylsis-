# kickstarter-anaylsis-
performing analysis on Kickstarter data to uncover trends 

## Overview 


The purpose of the project is to analyze the fundraising Louise has hold. Since the play Fever collected the goal amount in the short period of the time, to have the knowledge of relation between launched date and goal will benefit her greatly in the future. The report discusses results informative and simple by visualizing in charts. It creates the cognitive information of complicated data for the future success.  

## Analysis 

I used Countif() function to calculate the numbers of successful, failed and canceled. For example, I used,

=COUNTIFS(Kickstarter!D:D,"<1000",Kickstarter!R:R,"plays",Kickstarter!F:F,"Successful") 
to draw out successful plays on goal amount less than 1000. 

Also to calculate the percentage rate, I used IFERROR(ROUND) function to calculate the rate. For example I used,

=IFERROR(ROUND(B2/E2*100,0),0)

For the same goal amount. 

<img width="290" alt="Screen Shot 2022-03-13 at 7 28 29 PM" src="https://user-images.githubusercontent.com/100255000/158084382-899d973d-2aa3-4fe7-82a0-320bdcdc07a2.png">
 
For the pivot table, by putting goals for the rows and percentages on the values, I could create the table. And by using the table, I created the chart based on it. 

There was a challenge for the percentage section, I simply used dividing function and Instead of IRERROR, which gave me incorrect numbers on my pivot chart. I overcame it with re-reading the module to find out what I can do to resolve it. 


## Results 
o	What are two conclusions you can draw about the Theater Outcomes by Launch Date?

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/100255000/158084392-5e6124eb-48a5-4261-a0f1-ae7a4702e38c.png)


On the Chart, it shows two significant information. The successful event counts is spikes on May. It slowly decreases over through summer and increases a little bit on October and continues slopping down through December. On the other hand, Failed events has relatively stay in a flat line, spikes a little on October. Through this analysis, we can know that on the future year, we expect to see more successful events in spring and summer, and relatively not good in fall and winter time. 

o	What can you conclude about the Outcomes based on Goals?

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/100255000/158084398-777f337c-b0b8-4bdc-bf53-bb794a1fbfd7.png)


First of all, we can know that the plays that have goal of 25000 to 29999 failed second most. It also is the median value of the goals. The goal of 45000 to 49999 has the lowest successful rate. On the other than, the successful rate is highest at the lowest goal set which is less than 1000 dollars.

o	What are some limitations of this dataset?

Since, we only analyzed Theater and Play part of the whole fundraising data set, we lack of information other group. Only focusing on the subcategory part of the would not represent the whole situation of the fundraising.  

o	What are some other possible tables and/or graphs that we could create?

We could Create each charts and table of parent categories and sub-categories, instead having Play and Theater related charts. Instead, we can create matching charts for the monthly and goal outcome charts for Play to see where and when she can invest the fundraising. 
