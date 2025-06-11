# Advanced DAX

> DAX is simple, but it is not easy. *Alberto Ferrari*

For an introduction course we only touch on the simplest concepts in DAX so these are the advanced parts for this course, DAX goes way more advanced that this but thats a different course.

## Calculate Function

When you need to do a calculation filtered or changed in a particular way we use the CALCULATE function. This can be a filter, different relationships or a time intelligence filter.

* [CALCULATE function - Microsoft](https://learn.microsoft.com/en-us/dax/calculate-function-dax)
* [CALCULATE function - SQLBI](https://dax.guide/calculate/)


## Use inactive Relationships

When 2 tables have an inactive relationship that is required for a calculation, such as counting orders made vs orders delivered.

* [Using Inactive Relationships - Laura GB](https://hatfullofdata.blog/power-bi-inactive-relationships-in-a-measure/)
* [Use Rela](https://dax.guide/userelationship/)

## This Year Compared to Last Year - Time Intelligence

When you have data that covers multiple years a useful measure is to compare to last year and other time intelligence functions. SAMEPERIODLASTYEAR is the simplest function in the time intelligence family.

* [Time intelligence Functions - Microsoft](https://learn.microsoft.com/en-us/dax/time-intelligence-functions-dax)
* [SAMEPERIODLASTYEAR - Microsoft](https://learn.microsoft.com/en-us/dax/sameperiodlastyear-function-dax)
* [SAMEPERIODLASTYEAR - SQLBI](https://dax.guide/sameperiodlastyear/)