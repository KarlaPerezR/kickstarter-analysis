# An Analysis of Kickstarter Campaigns

## Overview of Project

### Analyze fundraising campaigns for plays according to their release dates and funding goals

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The plays that are most successful are in May, from this peak there is a downward behavior until the end of the year. <br/>
The plays that have failed the most have been in October.
<br/><br/>
![Outcomes_Date](https://github.com/KarlaPerezR/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
Most of the successful plays are related to small Goals (less than 5,000), while the plays with the highest goals in the market (45,000 and up) have a high percentage greater than 88% of failures.<br/><br/>
![Outcomes_Goals](https://github.com/KarlaPerezR/kickstarter-analysis/blob/main/resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

#### 1. How to group the date in Months in a Pivot Table

To group a date Field in months, I used to deleted from "Rows" the options "Años" and "Trimestres" so the Table Pivot could show Months
<br/><br/>![Row _Options](https://github.com/KarlaPerezR/kickstarter-analysis/blob/main/resources/Row_date_Options.PNG)
<br/><br/> But I found a new and easier way to group the field "Date Created Conversion" for the Pivot table at [Microsoft Support - Group](https://support.microsoft.com/es-es/office/agrupar-o-desagrupar-datos-en-una-tabla-din%C3%A1mica-c9d1ddd0-6580-47d1-82bc-c84a5a340725) by a right clicking over a date in the Table Pivot, Excel shows the options to "Group" or even "Ungroup"
<br/><br/> ![Group_monthly](https://github.com/KarlaPerezR/kickstarter-analysis/blob/main/resources/Group_Monthly.PNG)

#### 2. The translate of the Formula COUNTIFS los rangos de filtros
I struggle a little with the Formula of =COUNTIFS() because I have Excel in the Spanish version so at the beggining I was using the Formula =CONTAR.SI, but I saw that the video on Canvas has a different Syntaxis and founded the correct one, =CONTAR.SI.CONJUNTO() also at [Microsoft Support - COUNTIFS](https://support.microsoft.com/es-es/office/funci%C3%B3n-contar-si-conjunto-dda3dc6e-f74e-4aee-88bc-aa8c2a866842)
![Formula](https://github.com/KarlaPerezR/kickstarter-analysis/blob/main/resources/Formula_COUNT.png)

#### 3. The range for the Formula COUNTIFS
I write the formula of the Ranges using the value above the Requested range, p.e. I used "<20000" for the Range 15000 to 19999 instead that the option ">=19999".
This way of writting the formula make me doubt if the range was correct so I verified the counts with the filters manually in the sheet "Kickstarter".
<br/>In the future I will match the formula with the value in the range to avoid doubting.
<br/><br/>![Ranges](https://github.com/KarlaPerezR/kickstarter-analysis/blob/main/resources/Ranges.PNG)


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
<br/> Launch the play in May
<br/> Avoid the rest of the Year after May to launch a play and do not launched in October

- What can you conclude about the Outcomes based on Goals?
<br/>To have a successful play is recommended to be in a range of less than 5,000

- What are some limitations of this dataset?
<br/>The database has currencies from differents countries, so the data is not standardized.
<br/>The format of the Columns "Deadline" and "Launched_At" is in Unix Timestamps format, so you need to convert it.
<br/>The information is not updated, the most recent is from 2017.

- What are some other possible tables and/or graphs that we could create?
A graph to compare plays by countrys 
