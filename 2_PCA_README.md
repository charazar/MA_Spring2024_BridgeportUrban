**Project:** Bridgeport Urban   

**Node:** MA - Boston

**Term:** Spring 2024

**Team:** Silas Kirsch (Project Lead), John Hocknell, Maggie Roseto, Charlotte Tomlinson 

**Code Contact:** Charlotte Tomlinson, cbramwellt@gmail.com        

## Introduction  
This code is largely based on UHEAT 1.0, created by the Fall 2020 AZ DEVELOP team (see link below), a tool to analyze urban heat vulnerability, integrating sociodemographic and human factors as well as heat analysis. Our team had already completed an LST in GEE using code that Dr. Kenton Ross created, so we only used UHEAT 1.0 for our social vulnerability index. Slight adaptations had to be made to the code as we ran issues using the tidycensus package for the Principal Component Analysis. 

https://github.com/NASA-DEVELOP/UHEAT/tree/main 

## Applications and Scope   
Where will the code be used, and to what extent?   
This code will be used to combine important factors in configuring where to focus on modeling urban heat using Solweig, to create meaningful placements of a “Cool Corridors” Initiative 

## Capabilities 
The resulting code is used for block group level data for Bridgeport, CT, and is designed to expeditiously analyze the dimensions of heat vulnerability and identify the areas that require cooling intervention.

## Reccomendations
PCA is best run at the tract level due to the nature of ACS 5 year data. This also helps when adding other factors to the PCA, such as health data, because that is most often at the tract level. 
Our reccomendation is to adapt this code to the tract level, to better add more factors (i.e. Census data, transport data and health data) to your PCA. 

## Interfaces 
Socioeconomic data as written out by 
MA_Bridgeport_UDII_Spring2024_TidyCensus.R


### Languages
The only language this part of the project used is R. The end products are maps of social vulnerability that will be publicly distributed. (Use data resulting from GEE and TidyCensus packages in R 

### Packages
What other libraries or software packages does it rely on?  
"tidyverse","psych","paran","reshape2",
"tidycensus", "tigris","sf","ggpubr","MVN", 
"RColorBrewer", "pheatmap", "grid"

## Parameters
Describe any steps needed for the script to run. It will help to specify which line in the code will need to be changed by the user based on their needs. *(Still working on this)*


## Assumptions, Limitations, & Errors 
This is where limitations of the theory, model, science, etc should be briefly documented. If the tools only work for a specific scenario, say so.   *( still working on this as well)*

## Support
For relevant tutorials navigate to UHEAT README.
    https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Fraw.githubusercontent.com%2FNASA-DEVELOP%2FUHEAT%2Fmain%2F2020Fall_AZ_TempeUrb     anII_DraftCode_FD%2FFall2020_CodeTutorial_TempeUDII.docx&wdOrigin=BROWSELINK 

Contact Charlotte Tomlinson (cbramwellt@gmail.com) for specific questions related to code which deviates from the original UHEAT

Helpful Links: 

	Tempe Word Tutorial 
	https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Fraw.githubusercontent.com%2FNASA-DEVELOP%2FUHEAT%2Fmain%2F2020Fall_AZ_TempeUrb     anII_DraftCode_FD%2FFall2020_CodeTutorial_TempeUDII.docx&wdOrigin=BROWSELINK  
	
	Understanding Geographic Identifiers (GEOIDs)
      https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Fraw.githubusercontent.com%2FNASA-DEVELOP%2FUHEAT%2Fmain%2F2020Fall_AZ_TempeU       rbanII_DraftCode_FD%2FFall2020_CodeTutorial_TempeUDII.docx&wdOrigin=BROWSELINK  

	Spatial data in tidycensus  
     https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Fraw.githubusercontent.com%2FNASA-DEVELOP%2FUHEAT%2Fmain%2F2020Fall_AZ_TempeUr      banII_DraftCode_FD%2FFall2020_CodeTutorial_TempeUDII.docx&wdOrigin=BROWSELINK 

## Acknowledgments
Created by: Charlotte C. Wagner (ccwagner88@gmail.com)
Date created: March 10, 2020

Modified by: Blake A. Steiner (blake.a.steiner@gmail.com)
Date modified: Oct. 13, 2020

Modified again by: Charlotte B. R. Tomlinson

History:  2020, Mar 10 - ccw - adapted script from vulnerability-index.RMD
          2020, Mar 21 - ccw - added heat exposure and heat vulnerability index
          2020, Oct 13 - bas - modified code for just heat exposure index for Tempe 2020
          2020, Oct 25 - bas - modified code to take in new vulnerability variables for Tempe 2020
          2020, Oct 29 - bas - edited code to be neater
          2020, Nov 16 - bas - fixed row ordering issue in output
          2024, March 2- cbrt- adapted to block group level, only used heat vulnerability score, no use of heat exposure


