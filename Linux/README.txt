==LeafPy - An Automated Leaf Movement Tracking System==

by Mark Greenwood, Patrick Diaz, Amy Rothwell, Peter Gould, James Locke and Anthony Hall.
University of Liverpool & University of Cambridge.


==Introduction==

LeafPy is a system designed for low cost analysis of circadian leaf movement rhythms. It is designed to be affordable and easy to use for the non specialist.

The LeafPy system consists of two components: a time-lapse image capture and and a leaf tracking algorithm.


==Requirements==

LeafPy is developed in Python and distributed as executable files. It therefore has no installation or required dependencies. 

A reasonably modern PC should be used to run the program with a suggested minimum of 4GB RAM. It is recommended PCs with internal webcams should not be used. Alternatively, the internal webcam driver can be uninstalled prior to use.

On Windows, power saving settings should be set to ‘high performance’ and USB power saving disabled from the advanced settings. 

Web-cameras must be of 1080p resolution. Otherwise any model which supports your platform can be used. However, models with autofocus features should be avoided. Development was done using TeckNet 1080p Webcams (www.tecknetonline.com) and we recommend these. If a USB hub is required, it should be self powered. 


==Running LeafPy Image Capture==

Separate executable files are available for Windows and Unix platforms. You should download the folder relevant for your computer from the project GitHub.

All compatible webcams should be connect to the PC prior to running the program.

Image capture can be run by double clicking the ‘LeafPyCapture’ executable file in the relevant folder. On some platforms, the executable may need to be run through the command line.

Alternatively, the Python source files can be run directly but this will require the installation of several packages.

Once run, the user will be presented with a GUI allowing the selection of up to 16 webcams. You should select a different camera for each plate.

The webcam can be previewed using the ’test’ button. All the webcams should be focused by eye from a distance of approximately 5 inches.

The image should be framed so that each seedling fits inside a single square of the grid throughout the experiment. Growth and movement should be considered. This is important for the tracking stage.

Once all cameras are setup, the time interval and experiment length can be set and the program run. 


==Running LeafPy Tracking Analysis==

The Analysis program can be run as with the capture script. Run the ‘LeafPyAnalysis’ executable or Python file. 

In the command line, enter the directory of your images to be analysed. Images must have been obtained from the LeafPy Image Capture program.

Enter the plate positions used, comma delimited (e.g 1, 7, 15, 16).

Enter the time interval (seconds) and the number of time points in the experiment.

Allow the program to run. The results will be saved into a results folder inside the directory of images. Results consist of a graph of time versus leaf position for each seedling and an csv file containing the data. 

Data is formatted in a format appropriate for the popular time series data analysis system BioDare (www.biodare.ed.ac.uk).  


==Experimental set-up==

To facilitate automated analysis the experiment must be set-up in a standardised way. Seedlings should be prepared for imaging as described by Edwards et al., 2005; outlined here with some adaptations [1]:


	• Seeds are grown for 8 days in 12 h light/12 h dark (LD) cycles at 22 °C and 80 μmol m-2 		sec-1 constant white light.


 

 	• Plates are returned to growth conditions for one further day.




[1] Edwards KD, Millar AJ: Analysis of Circadian Leaf Movement Rhythms in Arabidopsis thaliana. 2007, 362:103–113.










