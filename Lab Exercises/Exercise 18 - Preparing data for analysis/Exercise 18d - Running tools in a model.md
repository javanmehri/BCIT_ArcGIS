# Running tools in a model

##### 1. Open the ex18d map document.

![](./img/ArcGis-18d-01.png)

##### 2. In the Catalog window, navigate to your MyData folder for chapter 18. Right-click MyData and click New > Toolbox.

![](./img/ArcGis-18d-02.png)

##### 3. In the Catalog window, change the new toolbox name to Oregon Forest Analysis and press Enter. In the Catalog tree, expand your MyData folder if necessary.

![](./img/ArcGis-18d-03.png)

Next, you will create a model within the toolbox.

##### 4. In the Catalog window, right-click the Oregon Forest Analysis toolbox and click New > Model.

![](./img/ArcGis-18d-04-1.png)

![](./img/ArcGis-18d-04-2.png)

##### 5. On the ModelBuilder menu bar, click Model > Model Properties.
##### On the General tab, in the Name box, replace Model with ForestAnalysis.
##### In the Lable box, replace Model with Forest Analysis. Click OK.

![](./img/ArcGis-18d-05-1.png)

![](./img/ArcGis-18d-05-2.png)

##### 6. On the ModelBuilder toolbar, click the Save button.

![](./img/ArcGis-18d-06.png)

##### 7. Close the ModelBuilder window.

##### 8. In the Catalog window, if necessary, click the plus sign (+) next to the Oregon Forest Analysis toolbox to open it and view the model inside.

![](./img/ArcGis-18d-08.png)

##### 9. On the Standard toolbor, click the ArcToolbox button. 

![](./img/ArcGis-18d-09.png)

##### 10. In the Catalog window, click the Oregon Forest Analysis toolbox and drag it to the bottom of the ArcToolbox window.

![](./img/ArcGis-18d-10.png)

The Oregon Forest Analysis toolbox is automatically added and alphabetized with the other toolboxes.

##### 11. Close or hide the Catalog window, since it will no longer be needed.

##### 12. In the ArcToolbox window, click the plus sign (+) next to Oregon Forest Analysis to expand its contents. Right-click the Forest Analysis model and click Edit. 

![](./img/ArcGis-18d-12-1.png)

![](./img/ArcGis-18d-12-2.png)

##### 13. In the ArcToolbox window, expand the Analysis Tools > Extract toolset.

![](./img/ArcGis-18d-13.png)

##### 14. Click the Clip tool and drag it to the center of the model window.

![](./img/ArcGis-18d-14.png)

##### 15. Drag the Populated Jurisdictions layer to the model window and drop it directly on top of the Clip tool rectangle. A shortcut menu appears. Click Input Features.

![](./img/ArcGis-18d-15-1.png)

![](./img/ArcGis-18d-15-2.png)

##### 16. Drag the CountyWarningAreas selection layer to the model window and drop it directly on top of the Clip tool rectangle. A shortcut menu appears. Click Clip Features.

![](./img/ArcGis-18d-16-1.png)

![](./img/ArcGis-18d-16-2.png)

##### 17. Drag the CountyWarningAreas selection element to a position below the Populated Jurisdictions element so you can see both inputs.

![](./img/ArcGis-18d-17.png)

##### 18. Double-click the output element in the model currently labeled as populated_juristictions_Clip. In the resulting window, click the Browse button and navigate to the contents of MyOregonForest.gdb in your MyData folder for chapter 18. In the Name box, type PortlandPopJurs, and then click Save.

![](./img/ArcGis-18d-18-1.png)

![](./img/ArcGis-18d-18-2.png)

##### 19. Click OK to close the dialog box.

![](./img/ArcGis-18d-19-1.png)

![](./img/ArcGis-18d-19-2.png)

##### 20. Right-click the PortlandPopJurs output oval and click Add To Display so it will be turned on in the table of contents.

![](./img/ArcGis-18d-20.png)

##### 21. On the ModeBuilder toolbar, click the Run button to run the model.

![](./img/ArcGis-18d-21-1.png)

![](./img/ArcGis-18d-21-2.png)

##### 22. Close the progress report. Notice that after a process runs, drop shadows appear behind the model elements.

![](./img/ArcGis-18d-22.png)

The PortlandPopJurs layer is added to ArcMap.

##### 23. Turn off the Populated Jurisdictions layer. Open the PortlandPopJurs layer properties and change the symbology to match the orange color of the Populated Jurisdictions layer.

![](./img/ArcGis-18d-23.png)

##### 24. Save the model.

![](./img/ArcGis-18d-24.png)




