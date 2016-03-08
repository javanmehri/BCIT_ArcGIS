# Joining data by location

In this exercise you will create a spatial  join based to combine two spatial layer. Specifically, you want to create a spatial join base on a containment relationship between two polygon layers.

##### 1. Open the ex17c map document.

![](./img/ArcGis-17c-01.png)

##### 2. On the Standard toolbar, click the ArcToolbox button. Expand the Analysis Tools > Overlay toolset.

![](./img/ArcGis-17c-02-1.png)

![](./img/ArcGis-17c-02-2.png)

##### 3. Open the Spatial tool.

##### 4. On the Spatial Join dialog box:
##### Target Feature --> Wisconsin Counties
##### Join Feature   --> Wisconsin Food Deserts
##### Output Feature Class --> ...\MyData\MyWisconsin.gdb\CountyStats

![](./img/ArcGis-17c-04.png)

##### 5. For Join Operation, maintain the default of JOIN_ONE_TO_ONE.

![](./img/ArcGis-17c-05.png)

You may wonder why you are using the one-to-one option here. This isn't about cardinality. You have many food deserts that you want to join to each county; however, you want only one row returned for each target feature.

##### 6. Maintain the default for Keep All Target Features. This means even counties without food deserts will remain in the output feature class.

##### 7. In the Field Map of Join Features panel, scroll down until you see the TOTALPOP (Double) field. Right-click it and click Merge Rule > Sum.

![](./img/ArcGis-17c-07-1.png)

![](./img/ArcGis-17c-07-2.png)

The output will now show the sum of all populations that live within the food deserts in each county.

Notice that the default merge rule is "First". This means that when there are multiple join features that share space with a target feature, only the first attribute value will appear in the output table.

##### 8. So you can see the average percentage of those living in food deserts who have low access to grocery stores, change the PERCENT_LOWA_Pop merge rule to Mean. 

![](./img/ArcGis-17c-08.png)

##### Then, change the merge rule for the next nine fields, summing the numerical figures and averaging (mean) the percentages (those with field names that begin with PERCENT_).

##### 9. Change the Match Option to CONTAINS.

![](./img/ArcGis-17c-09.png)

The Count field - which tallies all join features within each target feature - will be added automatically to the target table.

##### 10. Click OK to run the Spatial Join tool. When the process is completed, the ouput layer is added to the map with a randomly chosen fill color.

![](./img/ArcGis-17c-10.png)

##### 11. Close ArcToolbox. Then move the Wisconsin Food Deserts layer to the top of the drawing order in the table of contents.

![](./img/ArcGis-17c-11.png)

##### 12. Open the attribute table of CountyStats. Notice the Join_Count field. Sort it by ascending order.

![](./img/ArcGis-17c-12.png)

##### 13. Scroll through the rows and note how many food deserts are in each county.

So you now have attribute from counties, census tracts data, and the food desert research all within one table.

##### 14. Scroll to the right. Notice that the counties that have Join_Count value of 0 have null values for census tract data and food desert data. If you select one of these rows, you can see on the map that the county has no food deserts.

![](./img/ArcGis-17c-14.png)

##### 15. Scroll farther to the right. The food desert attributes you are interested in begin with TOTALPOP (toal number of people who live in food deserts in each county). Sort the TOTALPOP field by descending order, and then scroll to the top of the table.

![](./img/ArcGis-17c-15.png)

##### 16. Examine the other food desert attributes.

##### 17. Close the table and clear any selections. Open the layer properties of CountyStats and click the Symbology tab.

![](./img/ArcGis-17c-17.png)

##### 18. Click Quantities > Graduated colors > Fields
##### Value --> LOWA_POP

##### 19. In the Classification frame, click Classify

![](./img/ArcGis-17c-19.png)

##### 20. On the Classification dialog box, in the Data Exclusion frame, click Exclusion.
##### On the Data Exclusion Properties dialog box, on the query tab, build the following query: LOWA_POP IS NULL.

![](./img/ArcGis-17c-20-1.png)

![](./img/ArcGis-17c-20-2.png)

##### 21. Next, click the Legend tab. Select "Show symbol for excluded data" check box, and set the symbol color to white. For Lable, type No food deserts.

![](./img/ArcGis-17c-21.png)

##### 22. Click OK to close the Data Exclusion Properties dialog box, and then click OK again to close the classification dialog box.

##### 23. Back on the Symbology tab, above the center panel, click the Lable tab and click Format Labels.

![](./img/ArcGis-17c-23.png)

##### 24. Change the number of decimal places to 1 and click OK.

![](./img/ArcGis-17c-24.png)

##### 25. Finaly click Ok on the layer Properties dialog box to apply the changes.

##### 26. Turn off Wisconsin Food Deserts. Rename CountyStats Low Access Population and rename the legend Total by County.

![](./img/ArcGis-17c-26.png)










