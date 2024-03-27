# Project Short Title 
**Project:** Bridgeport Urban    

**Node:** Massachusettes-Boston   

**Term:** Spring 2024

**Team:** Silas Kirsch (Project Lead), John Hocknell, Maggie Roseto, Charlotte Tomlinson 

**Code Contact:** John Hocknell, jdhocknell@gmail.com      

## Introduction  
	This code analyzes land surface temperature using Landsat 8 TIRS and Landsat 9 TIRS. Our project's
	focus is on Bridgeport, Connecticut, but the study area for this script includes all of Fairfield
	County in Connecticut. Landsat images are acquired for each year from 2013 to 2023 for the summer
	months (June 01 to September 30) and merged into one collection. A temporal median is used to find
	the average value of each pixel for every band in this entire collection of images. Then a spatial
	reducer is used to find the median surface temperature for our reference area which is the town of
	Fairfield. The median reference value is then subtracted from every pixel in the entire study area
	to obtain a difference-LST image.

## Applications and Scope   
This code is to be used to understand how earth observation satellites can inform the distribution of heat within Bridgeport CT. By creating Land Surface Temperature Rasters, this code will inform a heat assessment and heat vulnerability package, to be used to inform Groundwork Bridgeport's Cool Cooridors initiative. 

## Capabilities 
This code mosaics multiple Landsat imagery captures over a study period to find the median Land Surface Temperature for a specified area. It uses that information to compare the study area to a reference area to determine the difference in heat. This information can then be used to inform policy makers and stakeholders to implement cooling strategies as extreme heat can have dangerous health consequences. 

## Interfaces 
Google Earth Engine (GEE)

### Languages
JavaScript within GEE 

## Parameters
Describe any steps needed for the script to run. It will help to specify which line in the code will need to be changed by the user based on their needs.  (inlcude examples)

1. Lines 15-17: input geometry or shapefiles
2. Lines 20-21: designate study and reference areas  
3. Lines 31-52: establish the collections of Landsat images and what dates they will be acquired from, then merge them all into one collection

## Assumptions, Limitations, & Errors
Land Surface Temperature is limited because it is surface temperature and not air temperature, it does not account for felt temperature. In addition, temperatures may not be accurate due to the potential inclusion of clouds, and other artifacts that may not be detected via the mask. Landsat also has a spatial resolution of 30m, which limits its ability to capture smaller-scale temperature variations. Finally, Landsat has a revisit time of 16 days so therefore may not record the weather events of interest (such as heat waves).

## Acknowledgments 
Dr. Kenton Ross - NASA Langley Research Center 
