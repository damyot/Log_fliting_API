# Remove events with low frequency from dataset

The removeEventsLowFrequency functions removes the events from DataFrame whose frequency is lower than the frequency provided.

## Usage
``
removeEventsLowFrequency (DataFrame dataName, String eventName, Int frequency)
``

## Arguments
- `dataName` is the name of pandas dataframe we want to manipulate.
- `eventName` is the name of the event we want to group by.
- `frequency` is the threshold value that is used to filter out rows whose count is less than threshold.

## Return
Return a dataframe containing only events whose frequency is larger than threshold.

## Example
```
data=removeEventsLowFrequency(dataset,’event’,20).
```

This will remove all the events are not met the minimum frequency.