# UMap
Bathymetric Community Map - This plugin enables any user to transform a stack of digital bathymetric data terrain models into a bathymetric community map. 

**Objective:**

This extension will facilitate the visualization and use of bathymetric data for the general public. This extension will enable any user to transform a bathymetric data digital terrain model into a bathymetric community map.

**UMap Plugin process:**

1. Click on windows button and open the QGIS Desktop application. Note that the plugin has been tested for QGIS 3.32 Lima and higher.

![image](https://github.com/umap-iic/UMap/assets/170830041/b2a75e19-def2-420c-99b8-95c3e45677b3)


2. Goto plugins and click on Manage and install plugins in QGIS Desktop

![image](https://github.com/umap-iic/UMap/assets/170830041/950f307e-bb64-4ee5-b008-45148ed5b10d)


3. Select All and search “UMap” and install the plugin

![image](https://github.com/umap-iic/UMap/assets/170830041/8e296361-c9d1-49f4-b523-a090d83592f7)


4. Goto “Plugins” and click on UMap

![image](https://github.com/umap-iic/UMap/assets/170830041/8a28f75f-d995-4726-be1c-992457759274)


5. UMap plugin GUI

![image](https://github.com/umap-iic/UMap/assets/170830041/3981a827-e5f0-4f6b-9480-63f0b0a54dd3)


6. Please provide a vector file (polygon type) of the extent of the map compilation area. The map extent can be submitted as the extent of the map canvas, drawn directly on the canvas or calculated from a map layer.

![image](https://github.com/umap-iic/UMap/assets/170830041/e0001abc-103f-4aff-a49f-5fb7c1becf5a)


7. Compilation scale is selected based on map extent provided.

![image](https://github.com/umap-iic/UMap/assets/170830041/036696c8-96cf-46a6-9408-e7ee800a0f76)


8. Please provide a vector file (polyline type) of the shoreline for the map compilation area. The shoreline can be submitted as a file (Shapefile, GeoPackage, or GeoJSON), a service (WFS), or a map layer.

![image](https://github.com/umap-iic/UMap/assets/170830041/3f2c735d-aa4d-4cb9-9c12-76f678cebe2b)

![image](https://github.com/umap-iic/UMap/assets/170830041/1eaecdf6-9fab-4297-8fe7-09fd30bcf8f1)

![image](https://github.com/umap-iic/UMap/assets/170830041/dc5af2fa-855b-45b6-9067-7b2a3c24f5c8)

![image](https://github.com/umap-iic/UMap/assets/170830041/fc09be6a-d988-48d9-b72c-f774528c7865)


9. Please provide one or more digital bathymetric terrain model for the map compilation area. The digital bathymetric terrain model can be submitted as a file (GeoTIFF, Shapefile, GeoPackage, or GeoJSON), a service (WCS), or a map layer.

![image](https://github.com/umap-iic/UMap/assets/170830041/b6dd8f4b-d817-474d-817b-b3240d3f9851)


10. Please select “Depth Contours Smoothing” value and “Sounding Selection” value from the available dropdown list.

![image](https://github.com/umap-iic/UMap/assets/170830041/19fb845f-b464-4c26-a685-bcab782a5055)


11. Click on “Run” button to execute UMap plugin process.


![image](https://github.com/umap-iic/UMap/assets/170830041/3bd39695-3d47-460c-b3ef-a2bf4b38591d)

![image](https://github.com/umap-iic/UMap/assets/170830041/1eec489a-35fb-42cb-9adc-970e603b9b83)

12. After processing the plugin the below Community map layers are generated.

![image](https://github.com/umap-iic/UMap/assets/170830041/26d981b2-1869-4da5-8b4e-b7e104af7816)


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


