# DATA CLEANING WITH POWER QUERY EDITOR 
This project is to keep my hands busy and to solidify my skill in data cleaning using power query editor in Microsoft Excel.The dataset was downloaded from forsightbi.com.ng via this [link](https://t.co/LEmsmrGL7b).

## PREVIEW OF THE DATASET

Looking at the dataset, it is supposed to contain four columns.Order IdShip modeSegmentValue/sales
But these columns are badly structured. The first two rows of the dataset contain the segment and ship mode attributes, with the Order ID attributes placed directly under the first two rows of column A.
The main objective of this exercise is to prepare and restructure the data for analytical purposes.The transpose and unpivot features in PowerQuery are the main tools used in the transformation process.

## LOADING THE DATASET

I created a new Excel workbook (Cleaned_badly_structured_data) and then loaded the dirty data into the Power Query Editor. To do this,Go to the data tab in MS Excel.Click on Get Data.Click on From File.Click on From Excel Workbook and then choose the file.Click on Transform and Load to load the data into the power query editor.

## DATA CLEANING PROCESS
After loading the data into the power query editor, the first row gets promoted automatically as a header, and the data type changes as well. To undo this, delete those steps in Applied steps’ in the power query editor.
Since we have the first two rows containing the segment and ship mode attributes, transpose the entire dataset. By transposing the dataset, the two columns are repositioned into two separate columns; however, the OrderID gets pivoted and therefore needs to be unpivoted.
Delete the OrderID column since it contains null values; use the fill-down feature to fill down the segment column; and remove null values in the ship mode column.
Now use the first row at the header and select the segment and ship mode columns, and then unpivote the other columns.
 
 
