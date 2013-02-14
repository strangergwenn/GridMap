GridMap
========

Overview
--------

A mapping tool intented for level design. Once the setup is done, you can find events in a log file and print a density map over an existing picture.
This tool was developped for DeepVoid (http://deepvoid.eu).


Usage
--------

You can call the script this way : gridmap.py <event> <resolution>
<event> will specify the event name to be searched in log. Events have a specific format.
<resolution> will specify the size of the computing unit, defined in real-world units (those used in the log file).

The format used in log is the following : "DVL/SHOOT/X/-305.2567/Y/-1557.8965/Z/46.5563/EDL"
It starts and ends by specific markers DVL and EDL, starts with the event name ("SHOOT" here) then stores the X, Y, Z coordinates.

The input log file has to be named "Launch.log".
The input picture file is hardcoded.
The output file is saved with the _heatmap extension after the source image name.


Hardcoded parameters
--------

Anytime you change the original picture, you will have to edit the script.

xmin = X coordinate of the picture left, in real world units
xmax = X coordinate of the picture right, in real world units
ymin = Y coordinate of the picture bottom, in real world units
ymax = Y coordinate of the picture top, in real world units
logBase : log base to use in calculation
bendAmount : amount of color to draw over the picture, from 0 to 1
unrealToPixelRatio : size of a pixel, in real world units
sourceImage : PNG file to use as a picture reference


Contact, people, etc
--------

GridMap is developped by Gwennaël ARBONA.
In case of bugs, questions, requests, ideas, please use the message system on GitHub.

