# Transform in Power Query

## Connect to Excel Files on OneDrive or SharePoint

First part of any reporting is to load and transform data. For first exercises we use Excel files and store them in OneDrive or SharePoint and load the data from there. Guy in Cube do a great video to show you how

[Excel and OneDrive with Power BI For Collaboration - Guy in Cube](https://www.youtube.com/watch?v=t4TzHu8THoA)

Another method from Microsoft that doesn't include the ?web=1 part is here

[Use OneDrive for work or school links in Power BI Desktop - Microsoft](https://learn.microsoft.com/en-us/power-bi/connect-data/desktop-use-onedrive-business-links?wt.mc_id=DX-MVP-5003563)

## Pick Transform not Load

When you've picked the tables etc click Transform Data to open Power Query. If you click Load by mistake or later want to return to Power Query, on the Home ribbon in Power BI desktop click Transform data.

![Transform Data buttons](<Images/Transform Options.png>)

## Power Query Basics

Power Query is a great at doing the transforms to tidy up data and make it useable in Power BI desktop. Be aware it doesn't have Undo.

[Use Power Query Interface](https://learn.microsoft.com/en-us/power-query/power-query-ui)

For most data the most important activities in Power Query are to remove unwanted columns, filter out un-required data and make sure columns have the right data types.

* [Choose or Remove Columns - Microsoft](https://learn.microsoft.com/en-us/power-query/choose-remove-columns?wt.mc_id=DX-MVP-5003563)
* [Filter by Value - Microsoft](https://learn.microsoft.com/en-us/power-query/filter-values?wt.mc_id=DX-MVP-5003563)
* [Data Types - Microsoft](https://learn.microsoft.com/en-us/power-query/data-types?wt.mc_id=DX-MVP-5003563)

## Transform columns

Data in columns can be transformed in various ways. The transform ribbon includes groups of buttons for Text, Number and Date. Select a column and the right buttons will be active.

![Transform Ribbon](<Images/Transform Columns.png>)

Selecting actions will add steps to the query.

## Split Columns

Columns can split by delimiter, positions and by case change. 

[Splitting Columns - Microsoft](https://learn.microsoft.com/en-us/power-query/split-columns-delimiter)

Careful editing of the split column M code allows for naming of the columns rather than adding rename steps

![alt text](<Images/split columns names.png>)

## Adding Columns

The most easiest columns to add are conditional columns and custom calcs. For more complicated new columns its worth looking at column by example for ideas in what M can do.

* [Conditional Column - Microsoft](https://learn.microsoft.com/en-us/power-query/add-conditional-column)
* [Custom Columns - Microsoft](https://learn.microsoft.com/en-us/power-query/add-custom-column)
* [Column by Example - Microsoft](https://learn.microsoft.com/en-us/power-query/column-from-example)

Its worth having some understanding of some M, be aware though there are over 700 functions, its case sensitive and no-one likes writing it by hand .If the custom column formulas need explanation the documentation can be found here

[Power Query M Function Reference - Microsoft](https://learn.microsoft.com/en-us/powerquery-m/power-query-m-function-reference)

## Duplicating and Referencing Queries

Often queries will depend upon other queries for example converting a flat file into a set of dim and fact tables. Sometimes duplicating a query is the best solution for a back up or creating a new independent query.

[Reference vs Duplicate - Radacad](https://radacad.com/reference-vs-duplicate-in-power-bi-power-query-back-to-basics/)



## Loading Data into Power BI Desktop

When all the data transformations have been done click on Close and Apply on the Home ribbon. If this brings through tables you didn't want, return to Power Query, right click on the query name and un-tick Enable Load

![Close & Apply button and Enable load on the menu](<Images/Load data.png>)

## Best Practices

Renaming steps, adding comments and using parameters are some of the best practices recommended.

* [Best practices - Microsoft](https://learn.microsoft.com/en-us/power-query/best-practices)
* [Creating New Parameters](https://hatfullofdata.blog/power-query-creating-new-parameters/)