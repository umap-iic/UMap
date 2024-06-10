# UMap
Bathymetric Community Map - This plugin enables any user to transform a stack of digital bathymetric data terrain models into a bathymetric community map. 

**Objective:**

This extension will facilitate the visualization and use of bathymetric data for the general public. This extension will enable any user to transform a bathymetric data digital terrain model into a bathymetric community map.

**UMap Plugin process:**

1. Click on Windows button and open the QGIS Desktop application. Note that the plugin has been tested for QGIS 3.32 Lima and higher.

![image](https://github.com/umap-iic/UMap/assets/138620082/9643148e-4752-4e00-a0ea-e40e5bb9285e)


2. Goto Plugins and click on Manage and Install Plugins in QGIS Desktop.

![image](https://github.com/umap-iic/UMap/assets/138620082/fad379c0-f0e1-430a-b44b-0934eeebf525)


3. Select All and search “UMap” and install the plugin.

![image](https://github.com/umap-iic/UMap/assets/138620082/f2b89a2c-fffb-40d7-a94c-139db446f348)


4. Goto “Plugins” and click on UMap.

![image](https://github.com/umap-iic/UMap/assets/138620082/a6151f50-4f46-4600-b6cf-65e92a433fea)


5. UMap plugin GUI.

![image](https://github.com/umap-iic/UMap/assets/138620082/4e52eb20-f632-4a4b-b71a-822126bf825c)


6. Please provide a vector file (polygon type) of the extent of the map compilation area. The map extent can be submitted as the extent of the map canvas, drawn directly on the canvas or calculated from a map layer.

![image](https://github.com/umap-iic/UMap/assets/138620082/3bae963d-15e5-438f-a049-8448c3b5c796)

![image](https://github.com/umap-iic/UMap/assets/138620082/d7767327-9e54-4ea4-99ff-76fde4bd4398)


7. Compilation scale is selected based on map extent provided.

![image](https://github.com/umap-iic/UMap/assets/138620082/1f437992-5ee5-42fd-88e8-93f0a31a03c4)


8. Please provide a vector file (polyline type) of the shoreline for the map compilation area. The shoreline can be submitted as a file (Shapefile, GeoPackage, or GeoJSON), a service (WFS), or a map layer. In Canadian waters, NrCAN CanCoast - Marine Shoreline Version 3.0 can be used. 

![image](https://github.com/umap-iic/UMap/assets/138620082/2647cfe6-2f07-4b76-b598-419c121cfa7d)


9. Please provide one or more digital bathymetric terrain model for the map compilation area. The digital bathymetric terrain model can be submitted as a file (GeoTIFF, Shapefile, GeoPackage, or GeoJSON), a service (WCS), or a map layer. In Canadian waters, CHS NONNA Web Coverage Service (WCS) can be used.

![image](https://github.com/umap-iic/UMap/assets/138620082/409d67a9-a44e-4649-aae7-9bf31c1213c4)


10. Please select “Depth Contours Smoothing” value and “Sounding Selection” value from the available dropdown list.

![image](https://github.com/umap-iic/UMap/assets/138620082/34e58ef9-8514-451d-9dc7-96ad85e73b36)


11. Click on “Run” button to execute UMap plugin process.

![image](https://github.com/umap-iic/UMap/assets/138620082/7c67c400-ee4e-4b36-802b-42b14935c465)


12. After processing the plugin the below Community map layers are generated.

![image](https://github.com/umap-iic/UMap/assets/138620082/f9a499c9-0a6b-4065-9805-6d82b17445d6)


**UMap plugin output layers:**

**Soundings:**

Sounding selection is a choice of critical, significant and representative depths.

**Shoreline:**

The region where the water bodies such as lakes, seas, and oceans meet the land. It can also be considered the boundary between the land surface and water bodies.

**Bathymetric contours:**

Bathymetric contours connect depths of the same value along a polyline. There are 8 bathymetric contour values (0m, 2m, 5m, 10m, 20m, 30m, 50m, 100m). The depth value of a contour must be transferred regularly along the polyline.

**Land areas:**

Land areas are those that are never covered by water. They fill in all the areas delimited by portions of shoreline closed in on themselves (islands) or closed off from the boundaries of the area to be mapped.

**Depth areas:**

Depth areas group together within a polygon all the depths of a given interval. There are 8 depth area intervals (<0m; 0m-2m; 2m-5m; 5m-10m; 10m-20m; 20m-30m; 30m-50m; 50m-100m).

**No Data areas:**

No Data areas represent areas for which no bathymetric data is available.

**Temporary files:**

Temporary files are created in C:\Temp\ folder. A dedicated folder for each process named UMapProcessingddmmaaaahhmmss (for example: UMapProcessing10062024151758) is created each time UMap is launched. This folder contains all the temporary and final files.

