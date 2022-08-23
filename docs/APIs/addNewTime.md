#  Transform time format

The addNewTime function will transform time column and create a new column called new_time to better manage time for the event logs. 
>In general,  user does not need to call this function explicitly because it is already called in the readCSV function. It is worth noting that when the time of the dataset does not follow regular timestamp, we can use this function to specify the timestamp formats.

## Usage
``
addNewTime (DataFrame dataName, String timeColName, String formats)
``

## Arguments
- `dataName` is the name of Pandas DataFrame we want to manipulate.
- `timeColName` is the name of the time column in the CSV file.
- `formats` is the format of time stamp. The default one is “%d%m%Y   %H: %M:%S”. The user can modify it according to the datasets.

## Return
Return a new DataFrame with new column ‘new_time’.

## Example
```
data=addNewTime (dataset, “time”,”%d%m%Y %H:%M:%S”).
```
