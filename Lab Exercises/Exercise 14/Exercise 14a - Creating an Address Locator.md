# Creating an Address Locator

The process of creating map features from addresses, place-names, and similar information is called **geocoding**.

Geocoding requires:
- an address table
- reference data ( To find the location of address points) 
- an address locator

An address locator is a file that contains the refrence data and various geocoding rules and tolerances (which are defined by an address locator style)

##### 1.Open the ex14a map document.

![](./img/ArcGis-14a-01-1.png)

![](./img/ArcGis-14a-01-2.png)

##### 2. At the top of the table of contents, click the List By Source button.

![](./img/ArcGis-14a-02.png)

##### 3. Open the School table.

![](./img/ArcGis-14a-03-1.png)

![](./img/ArcGis-14a-03-2.png)

##### 4. Open the table for the Philadelphia streets layer.

![](./img/ArcGis-14a-04-1.png)

![](./img/ArcGis-14a-04-2.png)

The attributes in the streets table most closely match the **US Address-Dual Ranges** addresss locator style. 

##### 5. Open the Catalog window in ArcMap.

##### 6. Navigate to \Chapter14\MyData. Right-click MyData and click New > Address Locator.

![](./img/ArcGis-14a-06-1.png)

![](./img/ArcGis-14a-06-2.png)

##### 7. Click the Browse button next to the Address Locator Style box. Choose US Address-Dual Ranges, and click OK.

![](./img/ArcGis-14a-07.png)

The Dual Range style is used for address ranges tath have data for both sides of a street segment. 

##### 8. Click the Reference Data box drop-down arrow and choose Philadelphia streets. 

![](./img/ArcGis-14a-08.png)

##### 9. Scroll down to view the Field Map list.

![](./img/ArcGis-14a-09.png)

##### 10. Click the Browse button next to the Output Address Locator box. Save it as Philadephia School in MyData Folder.

![](./img/ArcGis-14a-10.png)

##### 11. Click Ok To create the address locator.

![](./img/ArcGis-14a-11.png)

![](./img/ArcGis-14a-12.png)


