# Created isRepeated Column

This function created a new column called isRepeated for dataframe. It indicates whether the repeated or not. Please be noticed this function will automatically sort the rows by id and time.
>Please be noticed this function should run after ArrangeRows() function.For speed and efficiency, you can use this function to avoid duplicate sorts.

## Usage
``
eventIsRepeated (DataFrame dataset, String idName, String eventName)
``

## Arguments
- `dataName` is the name of pandas dataframe we want to manipulate.
- `idName` is one of column names we want to sort by and group by.
- `eventName` is one of column names.

## Return
Return a dataframe containing a new column called isRepeated.

## Example
```
data= eventIsRepeated (dataset, “case_id”,” event”]).
```