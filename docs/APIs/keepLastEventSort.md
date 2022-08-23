# Keep last event and drop repeated rows

This function removes the duplicated rows and keeps the last occurrence of an event. 
>Please be noticed this function will automatically sort the rows by id and time.

## Usage

``
data= keepLastEventSort (dataset, “event”,”case_id”])
``

## Arguments
- `dataName` is the name of pandas dataframe we want to manipulate.
- `idName` is one of column names we want to sort by and group by.
- `eventName` is one of column names.

## Return
Return a dataframe with only the last occurrence of an event name that is specified.

## Example
```
data= keepLastEventSort (dataset, “event”,”case_id”])
```