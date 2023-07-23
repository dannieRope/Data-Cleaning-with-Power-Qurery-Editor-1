# DATA CLEANING WITH POWER QUERY EDITOR 
The purpose of this project is to keep my hands busy and to consolidate my skill in data cleaning using power query editor in Microsoft Excel. The dataset was downloaded from forsightbi.com.ng via this [link](https://t.co/LEmsmrGL7b).

## PREVIEW OF THE DATASET

According to the dataset, it should have four columns: OrderId, Ship mode, Segment and Value/sales
However, these columns are poorly structured. Segment and ship mode attributes are found in the first two rows of the dataset, followed by Order ID attributes directly placed under them in column A.
The main objective of this exercise is to prepare and restructure the data for analytical purposes. Transpose and unpivot features in PowerQuery are the main tools used during the transformation.

## LOADING THE DATASET

I created a new Excel workbook (Cleaned_badly_structured_data) and then loaded the dirty data into the Power Query Editor. To do this,Go to the data tab in MS Excel.Click on Get Data.Click on From File.Click on From Excel Workbook and then choose the file.Click on Transform and Load to load the data into the power query editor.

## DATA CLEANING PROCESS
After loading the data into the power query editor, the first row gets promoted automatically as a header, and the data type changes as well. To undo this, delete those steps in Applied steps’ in the power query editor.
Since we have the first two rows containing the segment and ship mode attributes, transpose the entire dataset. By transposing the dataset, the two columns are repositioned into two separate columns; however, the OrderID gets pivoted and therefore needs to be unpivoted.
Delete the OrderID column since it contains null values; use the fill-down feature to fill down the segment column; and remove null values in the ship mode column.
Now use the first row at the header and select the segment and ship mode columns, and then unpivote the other columns.
 
 