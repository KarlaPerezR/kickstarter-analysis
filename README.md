# An Analysis of Kickstarter Campaigns

## Overview of Project

### Analyze fundraising campaigns for plays according to their release dates and funding goals

## Analysis and Challenges: 

### Analysis of Outcomes Based on Launch Date
#### The Campaigns
![Outcomes_Date](https://github.com/KarlaPerezR/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
![Outcomes_Goals](https://github.com/KarlaPerezR/kickstarter-analysis/blob/main/resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

#### How to group the date in Months in a Pivot Table

To group a date Field in months, I used to deleted from "Rows" the options "Años" and "Trimestres" so the Table Pivot could show Months
<br/>![Row _Options](https://github.com/KarlaPerezR/kickstarter-analysis/blob/main/resources/Row_date_Options.PNG)
<br/> But I found a new and easier way to group the field "Date Created Conversion" for the Pivot table at [Soporte de Microsoft](https://support.microsoft.com/es-es/office/agrupar-o-desagrupar-datos-en-una-tabla-din%C3%A1mica-c9d1ddd0-6580-47d1-82bc-c84a5a340725) by a right clicking over a date in the Table Pivot, Excel shows the options to "Group" or even "Ungroup"
<br/> ![Group_monthly](https://github.com/KarlaPerezR/kickstarter-analysis/blob/main/resources/Group_Monthly.PNG)

#### La traducción de la formula, filtrar de acuerdo a las plays, los rangos de filtros

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
<br/> en Mayo se tienen las obras más existosas
<br/>mientras que de oct a dic hay una tendencia a la baja en la obras cexitosas 

- What can you conclude about the Outcomes based on Goals?
<br/>la mayoría de las obras existosas estan relacionado a tamaños de metas pequeños (menores a 5,000), mientras que las obras con las metas más altas del mercado (45,000 en adelante) tienen un alto porcentaje mayor al 88% de fracasos 
para tener exito una obra debe de estar en un rango menor a los 5,000

- What are some limitations of this dataset?
Currency, tipo de cambio no indicado
el formato del Deadline y Launched_At en Unix Timestamps
información desacutualizada, lo más actual es del 2017

- What are some other possible tables and/or graphs that we could create?
Yes, we can compare the years more successful
also filter by the countrys of interest
