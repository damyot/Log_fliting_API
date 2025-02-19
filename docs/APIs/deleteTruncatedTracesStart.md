# Remove truncated traces

This function removes the traces that do not start with the provided eventName. 
>Please be noticed this function should run after ArrangeRows() function.For speed and efficiency, you can use this function to avoid duplicate sorts.

## Usage
``
deleteTruncatedTracesStartSort (DataFrame dataset, String idName, String eventName, String startEvent)
``

## Arguments
- `dataName` is the name of pandas dataframe we want to manipulate.
- `idName` is one of column names we want to sort by and group by.
- `eventName` is one of column names.
- `startEvent` is the value of event’s name required to start with.

## Return
Return a dataframe containing only traces started with specified event.

## Example
```
data= deleteTruncatedTracesStartSort (dataset, “case_id”,”event”,”Home page”]).
```
In this example, the function will remove all the traces that do not start with 
“Home page” event. It will help us filter incomplete traces whose beginning was not started with begin event.
