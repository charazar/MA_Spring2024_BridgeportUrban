# MA_Spring2024_BridgeportUrban
1_GEE_README
File: 	1_Spring2024_Bridgeport_Retrieve_LST_GEE.txt
Name: 	Urban Heat Land Surface Temperature Analysis
Author: Dr. Kenton Ross, NASA Langley Research Center
	adapted by Spring 2024 Bridgeport Urban Development
Description:
	Analyzes the difference in land surface temperature between a study area and a reference area 
	for a study period. In this project, the study area is Fairfield County, CT. The reference area
	is the town of Fairfield, just next to Bridgeport which is the focus of the project. The study 
	period is the summer months (June 01 to September 31) from 2013 to 2023. Images for this period
	are taken from Landsat 8 & 9 and merged into one image collection. The median of this image 
	collection is found for each pixel and band. Then a spatial reducer is used to find the median 
	surface temperature for the reference area. This value is subtracted from every pixel in the
	entire study area to obtain a difference-LST image. Shapefiles are imported from shared assets in 
	GEE.
