# Read a CSV file

The readCSV functions reads the CSV file into a Pandas DataFrame. And for subsequent use of the time filtering functions, we need to introduce the time column name in advance and transform it. This function read the csv file and create a new Column called ‘new _time’.

## Usage
``
readCSV (String fileName, String timeColName)
``

## Arguments
- `filename` is the name of the CSV file we want to import.
- `timeColName` is the name of the time column in the CSV file.

## Return
Returns a Pandas DataFrame.

## Example
```
data=readCSV(dataset,'TimeStamp')
```
This will read the CSV file under the current path to the Pandas dataframe which has been created called data. Table1 below an example of a source dataset file. The first column is the attributes’ name of each of event logs. Table2 gives an example what column the readCSV will create for us.

Table 1: An example of source dataset

| Case.ID 	| TimeStamp           	| event                   	| City     	| Client           	| Product_Category 	| Device  	|
|---------	|---------------------	|-------------------------	|----------	|------------------	|------------------	|---------	|
| ...     	| ...                 	| ...                     	| ...      	| ...              	| ...              	| ...     	|
| 121     	| 08/01/2018 00/07/00 	| Click Home Page         	| Ottawa   	| Computer Browser 	| A                	| Android 	|
| 122     	| 08/01/2018 00/07/02 	| Confirmation Order Page 	| Toronto  	| Phone App        	| B                	| Apple   	|
| 121     	| 08/01/2018 00/07/03 	| Add to Cart             	| Ottawa   	| Computer Browser 	| N/A              	| Andriod 	|
| 123     	| 08/01/2018 00/07/04 	| Review Shopping Cart    	| Waterloo 	| Phone App        	| A                	| Apple   	|
| ...     	| ...                 	| ...                     	| ...      	| ...              	| ...              	| ...     	|

Table 2: Pandas DataFrame after using readCSV () function

| Case.ID 	| TimeStamp           	| event                   	| City     	| Client           	| Product_Category 	| Device  	| new_time 	|
|---------	|---------------------	|-------------------------	|----------	|------------------	|------------------	|---------	|----------	|
| ...     	| ...                 	| ...                     	| ...      	| ...              	| ...              	| ...     	| ...      	|
| 121     	| 08/01/2018 00/07/00 	| Click Home Page         	| Ottawa   	| Computer Browser 	| A                	| Android 	| 420      	|
| 122     	| 08/01/2018 00/07/02 	| Confirmation Order Page 	| Toronto  	| Phone App        	| B                	| Apple   	| 422      	|
| 121     	| 08/01/2018 00/07/03 	| Add to Cart             	| Ottawa   	| Computer Browser 	| N/A              	| Andriod 	| 423      	|
| 123     	| 08/01/2018 00/07/04 	| Review Shopping Cart    	| Waterloo 	| Phone App        	| A                	| Apple   	| 424      	|
| ...     	| ...                 	| ...                     	| ...      	| ...              	| ...              	| ...     	|          	|