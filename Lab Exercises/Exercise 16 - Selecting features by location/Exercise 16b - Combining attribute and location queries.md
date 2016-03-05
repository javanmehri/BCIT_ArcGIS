# Combining attribute and location queries

##### 1. Open the map document.

In this exercise, you will select parcels that zoned residential (an attribute query) and that intersect the flood zone (a location query). 

![](./img/ArcGis-16b-01-1.png)

![](./img/ArcGis-16b-01-2.png)

This map shows the results of ex. 16a, through step 7. The Guerneville parcels that intersect the flood zone have been selected.

##### 2. Active "Select By Attribute" dialog box.

![](./img/ArcGis-16b-02.png)

##### 3. Do these settings:
##### Layer --> Gueneville Parcels
##### Method --> Select from current selection

![](./img/ArcGis-16b-03.png)

##### 4. In the fields list, double-click "BASEZONING" to add it to the expression box. Click the equals sign (=) to add it to the expression.

##### 5. Click Get Unique Values. The values for the BASEZONING field are listed.

##### 6. In the list of values, double-click 'Residential' to add it to the expression. Click OK to make the selection.

![](./img/ArcGis-16b-06-1.png)

![](./img/ArcGis-16b-06-2.png)

The selection now indicates parcels that are within the flood zone and zoned as residences. 

##### 7. Open the attribute table of Guerneville Parcels.

![](./img/ArcGis-16b-07-1.png)

![](./img/ArcGis-16b-07-2.png)

See how many parcels are currently selected.

Next, you will save the selection as a new layer.

##### 8. In the table of contents, right-click Guerneville Parcels > Selection > Create Layer From Selected Features.

![](./img/ArcGis-16b-08.png)

##### 9. Close the attribute table, clear the current selection, and turn off Guerneville Parcels.

![](./img/ArcGis-16b-09-1.png)

![](./img/ArcGis-16b-09-2.png)

##### 10. Change the default polygon symbol for the new layer. Use a hollow fill (no clolor) and a red outline, and then click OK.

![](./img/ArcGis-16b-10-1.png)

![](./img/ArcGis-16b-10-2.png)

##### 11. Zoom to the Guerneville2 bookmark and turn off the flood zone layer.

![](./img/ArcGis-16b-11-1.png)

![](./img/ArcGis-16b-11-2.png)

![](./img/ArcGis-16b-11-3.png)



