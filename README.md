# Imaginal-Disc-Profile
This script is a desinged to run as a macro in ImageJ. It quantifies the pixel intensity accross an epithelial section.

To use:
Place in a folder together: ImageName_Curve_Script.ijm, your image of interest
Open your image of interest in ImageJ
Using the line segment tool, select "Freehand Line"
Trace the apical part of your epithelium on the image
Go to file> Save As> XY Coordinates
Name this file [the same name as your image]_outer
  For example, if image name is RedChannel, name the file RedChannel_outer
Draw a line segment tracing the basal part of your epithelium, and save file as [the same name as your image]_inner

In your folder you should now have:
ImageName_Curve_Script.ijm
your image of interest
[imagename]_inner
[imagename]_outer

Go to Plugins> Macros> Run and select ImageName_Curve_Script.ijm
This should give the quntification of pixel intensities accross the epithelium, binned by ROIs which will appear on screen
Lines may be redrawn to better fit the tissue
To adjust the number of ROIs, ImageName_Curve_Script.ijm may be edited 
  In line3, set ndivis = to the number of desired ROIs. Default is 100 
