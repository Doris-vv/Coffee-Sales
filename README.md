# Coffee Sales Project - Excel & Tableau & Powerpoint
Watch this presentation on Linkdin at

The raw data for this project is presented in 3 sheets of 1 CSV file. This data represents coffee sales order, and they need to answer a few questions which will help them make important decisions to increase sales and improve their business.

The project is done in excel and tableau and presented in PowerPoint.

## Data Source
You can find the file in the repository.

## Tools
|Tool        |Purpose                                                                        |
|------------|-------------------------------------------------------------------------------|
|Excel  |Cleaning and transforming the data                                       |
|Mokkup AI   |Designing the wireframe/mockup of the dashboard                                |
|Tableau    |Visualizing the data via interactive dashboards                                |
|PowerPoint       |Present the insight and action plan|
|GitHub      |Hosting the project documentation and version control                          |

## Data Transforming with Excel
There are 3 sheets, the data can be transformed into 1 sheet through dax measures.
#### The column of Customer Name, Email, Country, City and Loyalty Card
```
XLOOKUP(C2,customers!A:A,customers!G:G)
```
#### The column of Coffee Type, Roast Type, Size and Unit Price
```
@INDEX(products!$A:$G,MATCH($D2,products!$A:$A,0),MATCH(J$1,products!$A$1:$G$1,0))
```
#### The column of Coffee Type Name and Roast Type Name
```
IF(J2="Rob","Robusta",IF(J2="Exc","Excelsa",IF(J2="Ara","Arabica",IF(J2="Lib","Liberica",""))))
IF(K2="M","Medium",IF(K2="L","Light",IF(K2="D","Dark","")))
```

## Data Visualization

## Findings
1.The busiest days are Wedesday and Saturday. The most leisure day is Thursday.
2.Arabica is the most popular coffee type.
3.Most people choose the 0.5kg size coffee.
4.More than half people don't use Loyalty Card.

## Conclusion
The outlet should capitalize on 0.5kg Aribica coffee, and give more discounts and sell different types of coffee to attract more people using Loyalty Card.
