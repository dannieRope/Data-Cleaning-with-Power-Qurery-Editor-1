# DATA CLEANING WITH POWER QUERY EDITOR 
The purpose of this project is to keep my hands busy and to consolidate my skills in data cleaning using the power query editor in Microsoft Excel. The dataset was downloaded from forsightbi.com.ng via this [link](https://t.co/73HKlw0xuI) 

## PREVIEW OF THE DATASET

According to the dataset, it should have four columns: OrderId, Ship mode, segment, and Value/sales.

However, these columns are poorly structured. Segment and ship mode attributes are found in the first two rows of the dataset, followed by Order ID attributes directly placed under them in column A.

![DATA PREVIEW](https://github.com/dannieRope/Data-Cleaning-with-Power-Qurery-Editor-1/assets/132214828/f4ac042a-50af-4ecd-8835-8d741a5a575a)


The main objective of this exercise is to prepare and restructure the data for analytical purposes. The transpose and unpivot features in PowerQuery are the main tools used during the transformation.

## LOADING THE DATASET

To load the dirty data into power query editor, create a new Excel workbook (Cleaned_badly_structured_data) and then; 

*Click the data tab in MS Excel.*

*Click on Get Data.*

*Click on From File.*

*Click on From Excel Workbook and then choose the file.*

![from excel workbook](https://github.com/dannieRope/Data-Cleaning-with-Power-Qurery-Editor-1/assets/132214828/cb7e499e-18b3-453a-83e5-3a12ca366f7e)

*Click on the excel sheet containing the dirty data*

*Click on Transform data to load the data into the power query editor.*

![Transform data](https://github.com/dannieRope/Data-Cleaning-with-Power-Qurery-Editor-1/assets/132214828/4884ad53-db60-4060-928b-865f6a068bdd)


## DATA CLEANING PROCESS

After loading the data into the power query editor, the first row gets promoted automatically as the headers, and the data type changes as well. To undo this, delete those steps in Applied Steps in the power query editor.

![undo](https://github.com/dannieRope/Data-Cleaning-with-Power-Qurery-Editor-1/assets/132214828/1f9d97b5-af0b-47d3-a39a-74c93c5f220f)


Since we have the first two rows containing the segment and ship mode attributes, transpose the entire dataset. By transposing the dataset, the two rows are repositioned into two separate columns. To transpose the dataset,
in the transform tab in the power query editor,
click on transpose

![transpose](https://github.com/dannieRope/Data-Cleaning-with-Power-Qurery-Editor-1/assets/132214828/40bde25e-ee52-4ad9-843b-89562a8d2fd6)


However, the OrderID column attributes become rows.

Delete the column named OrderID since it contains null values; to do this, right-click on the column and click on remove.

![remove](https://github.com/dannieRope/Data-Cleaning-with-Power-Qurery-Editor-1/assets/132214828/f3e028bf-9e99-4aac-9d77-8e77f9747bb2)


Use the fill feature to fill down the segment; to do this, In the transform tab, click on fill, choose down from the drop-down menu.

![fill down](https://github.com/dannieRope/Data-Cleaning-with-Power-Qurery-Editor-1/assets/132214828/928e56c5-677a-44cd-b46d-52d5d3b0e417)

Remove null values in the ship mode column. To do this, click on the drop-down button on the right side of the ship mode column and then click on Remove empty rows.

![remove empty](https://github.com/dannieRope/Data-Cleaning-with-Power-Qurery-Editor-1/assets/132214828/64a7694b-0e71-43b8-94c4-e6f73fcfdcb0)

Now use the first row at the header. To do this, click on use first rows as header in the transform tab

![use first row as header](https://github.com/dannieRope/Data-Cleaning-with-Power-Qurery-Editor-1/assets/132214828/47cf2a30-2e41-4782-988c-da16466fc650)

To get the OrderID column, Unpivot the dataset by first selecting the Segment and Ship Mode columns, and then, in the transform tab, click on the unpivot column and select unpivot other columns from the drop-down menu.

![unpivot](https://github.com/dannieRope/Data-Cleaning-with-Power-Qurery-Editor-1/assets/132214828/96edbd20-48e1-4ca6-9d76-8a078d4610c0)

Now change the attribute column name to OrderID by double-clicking the column header 

![u have it](https://github.com/dannieRope/Data-Cleaning-with-Power-Qurery-Editor-1/assets/132214828/f7ea541c-8da7-487f-b43e-bc9d35ef2100)


In the Home tab, click on close and load.

![close and load and save the excel sheet](https://github.com/dannieRope/Data-Cleaning-with-Power-Qurery-Editor-1/assets/132214828/39353717-d30c-488e-919d-9aa17ae7734c)


Save the excel sheet. 

Take a look at the clean dataset [here](https://github.com/dannieRope/Data-Cleaning-with-Power-Qurery-Editor-1/blob/main/1.Badly_structured_sales_Data_Cleaned.xlsx)

![final](https://github.com/dannieRope/Data-Cleaning-with-Power-Qurery-Editor-1/assets/132214828/0e013fb2-0b4c-4f5c-8713-42eb7a42af4e)




 
 
