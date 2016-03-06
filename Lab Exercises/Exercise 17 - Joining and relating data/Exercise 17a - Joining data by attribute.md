# Joining data by attribute

In this exercise we will examine the Food Access Research Atlas, a study to identify "food deserts", which are low-income neighborhoods with high concentrations of people who are far from a grocery store. 

##### 1. To examine the results of the Food Desert Locator study, go to this link address:

http://www.ers.usda.gov/data-products/food-access-research-atlas.aspx

![](./img/ArcGis-17a-01.png)

##### 2. Under Overview, read about the atlas, and then click "Enter the Map". 

![](./img/ArcGis-17a-02.png)

##### 3. Click any green square. scroll through the pop-up box and notice the information that is provided.

![](./img/ArcGis-17a-03.png)

##### 4. Above the map, click the About the Atlas link. Read the section titled "Overview" and "Measures of food access."

![](./img/ArcGis-17a-04-1.png)

![](./img/ArcGis-17a-04-2.png)

Next, you will learn how to create a similar map using an ERS dataset, limiting the study area to the state of Wisconsin.

##### 5. Open the ex17a map document.

![](./img/ArcGis-17a-05.png)

##### 6. Open the attribute of Wisconsin census tracts and examine the information. Notice the FIPS_TRACT field.

FIPS_TRACT --> a unique identification number for each census tract record.

![](./img/ArcGis-17a-06.png)

##### 7. Close the table.

##### 8. Start Excel and open FoodDesert_Data.xls from Data Folder.

![](./img/ArcGis-17a-08.png)

##### 9. Scroll down through the rows of Data. Notice that the spreadsheet indicates data for all 48 continental states. (Hawaii and Alaska weren't included in the study.)

##### 10. Scroll back to the top of the spreasheet. Now scroll across and examine the column headings. To decipher the abbreviations, click the variable_lookup tab at the bottom of the spreadsheet and read the variable descriptions.

![](./img/ArcGis-17a-10.png)

##### 11. Minimize Excel. In ArcMap, click the Add Data button. Navigate to Data folder, double-click FoodDesert_Data.xls, and click Data$. Then click Add.

![](./img/ArcGis-17a-11-1.png)

![](./img/ArcGis-17a-11-2.png)

##### 12. In the table of contents, right-click the Data$ table and click Open.

##### 13. Scroll down to find the data records for Wisconsin (Wl in the State). Notice that there are several tracts per county.

![](./img/ArcGis-17a-13.png)

##### 14. Right-click TRACT_FIPS, and on the shortcut menu, click Freeze/Unfreeze Column. Scroll all the way to the right.

![](./img/ArcGis-17a-14-1.png)

![](./img/ArcGis-17a-14-2.png)

For each record in the Wisconsin census tracts table, there is no more than one matching record in the FoodDesert_Data table, thus making a good choice for a join operation.

##### 15. Close the table. In the ArcMap table of contents, right-click Wisconsin Census Tracts > Joins and Relates > Join.

![](./img/ArcGis-17a-15.png)

##### 16. In the first drop-down list, make sure "Join attributes from a table" is selected. In the first entry box, select FIPS_TRACT.

##### 17. In the second entry box, make sure the Data$ table is selected. In the box 3, make sure the TRACT_FIPS field is selected.

##### 18. In the Join Options selection, you want to keep all the records.

![](./img/ArcGis-17a-18.png)

##### 19. Click OK, to run the join operation.

##### 20. Open the attribute table of the Wiscosin Census Tracts layer. Scroll to the right until you see the shape_area field.

![](./img/ArcGis-17a-20.png)

To the right of Shape_Area are the fields from the FoodDesert table, which are shown using field aliases. Field aloases are a more user-friendly description of the content of the field.

##### 21. Turn off the field aliases by clicking the Table Options button, and then click Show Field Aliases to cler the selection.

![](./img/ArcGis-17a-21-1.png)

![](./img/ArcGis-17a-21-2.png)

##### 22. Resize the Data$.TRACT_FIPS field to see its entire name.

![](./img/ArcGis-17a-22.png)

##### 23. Use the knowledge you gained in chapter 15 to perform a Select By Attributes query using this SQL statement:

##### "Data$.TRACT_FIPS" IS NOT NULL

![](./img/ArcGis-17a-23.png)

##### 24. Apply the selection, and then close the Select By Attributes dialog box. Show only the selected records in the attribute table.

![](./img/ArcGis-17a-24-1.png)

![](./img/ArcGis-17a-24-2.png)

##### 25. Move the table out of the way so you can see the map display. The selected records are also selected on the map.

![](./img/ArcGis-17a-25.png)

##### 26. Close the table. Tracts will remain selected on the map.

##### 27. In the table of contents, right-click Wisconsin Census Tracts and click Data > Export Data. 

![](./img/ArcGis-17a-27.png)

##### 28. For the output location, browse to your MyData folder for chapter 17. Click the save as type arrow and click File and Personal Geodatabase feature classes. Double-click MyWisconsin.gdb, and for Name, type FoodDeserts. Click Save.

![](./img/ArcGis-17a-28-1.png)

![](./img/ArcGis-17a-28-2.png)

![](./img/ArcGis-17a-28-3.png)

##### 29. Click OK to export the data. When the operation is complete, click Yes to add the new layer to the map.

![](./img/ArcGis-17a-29-1.png)

![](./img/ArcGis-17a-29-2.png)

##### 30. Clear the selected features. Change the table of contents to the Drawing Order view, and change the name of the new layer to Wisconsin Food Deserts.

![](./img/ArcGis-17a-30-1.png)

![](./img/ArcGis-17a-30-2.png)









