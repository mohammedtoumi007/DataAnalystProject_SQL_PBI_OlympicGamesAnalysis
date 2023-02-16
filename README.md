# DataAnalystProject_SQL_PBI_OlympicGamesAnalysis
Olympic Games Analysis

## Business Problem
The challenge for this data analyst project is outlined below. This has been used continuously to ensure that the right data has been selected, transformed and used in the data visualization which is meant to be passed on to the business users.

## Data Collection & Table Structures
The necessary data was first put into a SQL database and afterwards transformed using the transformations.

## Data Model
Where dimensions and facts have been combined, the data model that is created in Power BI is one table. The query from previous step was loaded in directly.

## Calculations : DAX 
The following calculations were created in the Power BI reports using DAX (Data Analysis Expressions). To lessen the extent of coding, the re-use of measures (measure branching) was emphasized:

Number of Competitors:
# of Competitors = DISTINCTCOUNT( ‘Olympic Data'[ID] )
# of Medals = COUNTROWS( ‘Olympic Data’ )
# Of Medals (Registered) = CALCULATE( [# of Medals], FILTER( ‘Olympic Data’, ‘Olympic Data'[Medal] = “Bronze” || ‘Olympic Data’ [Medal] = “Gold” || ‘Olympic Data'[Medal] = “Silver” ))

## Olympic Games Analysis Dashboard

The finished dashboard consist of visualizations and filters that gives an easy option for the end users to navigate the summer games through history. Some possibilities are to filter by period using year, nation code to focus on one country or look into either a competitor or specific sports over time.

![dashboard](https://user-images.githubusercontent.com/55878755/219421827-4759c342-5732-43d5-a1c2-410bcdc6b28a.png)

Link Dashboard : https://www.novypro.com/project/project-3
