# Modelling in Power BI desktop

Once you have connected to the data and completed you can start modelling. The main points in this section are

* Adding Measures
* Relationships
* Adding a calendar

## Adding Measures

The calculations such as counting rows, totalling a column should be done in measures. This gives us control on the naming, formatting and the power of DAX.

[Create measures in Power BI - Microsoft](https://learn.microsoft.com/en-us/power-bi/transform-model/desktop-measures)

The simplest measures include SUM, COUNTROWS and AVERAGE.

```
Total Revenue = SUM ( Sales[Revenue] )
```

Make sure measures have the right Home table and that each measure is formatted.

See the Advanced DAX mo


## Relationships

If you have more than one table in your report there is possibly a relationship between them. 

[Create and manage relationships in Power BI Desktop - Microsoft](https://learn.microsoft.com/en-us/power-bi/transform-model/desktop-create-and-manage-relationships)

### Note

Multiple relationships between tables mean only one will be active. Pick the most commonly used relationship to be active. See the Advanced DAX

Many to many relationships are a bad idea and should be avoided. Find ways to make relationships 1 to many or many to 1.

Bi directional joins are a bad idea and can lead to ambiguity this is explained by Alberto from SQLBI - [Bidirectional relationships and ambiguity in DAX](https://www.sqlbi.com/articles/bidirectional-relationships-and-ambiguity-in-dax/)