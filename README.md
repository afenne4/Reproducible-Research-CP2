# Reproducible Research-Economic and Public Health Consequences of Severe Weather Events
For this project, data from the U.S. National Oceanic and Atmospheric Administration’s (NOAA) storm database
was obtained and used to answer the questions of what severe weather events cause the most damage in relation
to the economy and public health. A simple exploratory data analysis was conducted to answer this question. 
There are almost 1 million observations across 37 variables (columns) in the dataset.

## Variables of interest
Of the 37 variables there are only 8 variables that are of interest for this analysis.
  
  -Date: A character string with the date in the format of MM/DD/YYYY with meaningless time
  (there is another variable that records the actual time) in the format of H:MM:SS
  
  -EVTYPE: A character string with labels for each severe weather event occurred. There are 48
  official event types ([Storm Data Documentation](https://d396qusza40orc.cloudfront.net/repdata%2Fpeer2_doc%2Fpd01016005curr.pdf)) but due to data entry discrepancies, there are many more unique instances
  than this. Details for how this was addressed are located in the .Rmd and .pdf files.
  
  -Fatalities: A numeric variable with counts of deaths resulting from a weather event.
  
  -Injuries: A numeric variable with counts of injuries resulting from a weather event.
  
  -PropDmg:A numeric variable containing information about the amount of property damage a 
  weather event causes (in USD)
  
  -PropDmgExp: A character variable that indicates PropDmg needs to get modified by a certain 
  amount. H=100 \* PropDmg, K=1000 \* PropDmg, M=10^6 \* PropDmg, B=10^9 \* PropDmg. 
  There are other values  but they only modify the last digit by a trivial amount, when damage 
  can be hundreds of millions of dollars.
  
  -CropDmg: A numeric variable containing information about the amount of crop damage a weather
  event causes (in USD).
  
  -CropDmgExp: A character variable that indicates CropDmg needs to get modified by a certain 
  amount. The modifications are the same as PropDmgExp, but are applied to CropDmg.

## Files in this Repo
The report showcasing the analysis of this data is located in the pdf file and contains the rendered figures
There is also the R Markdown file which can be used to independently run the analysis. These files are commented 
so the reader understands the code chunks and why certain data preparation decisions were made in addition to an 
interpretation of the figures.



