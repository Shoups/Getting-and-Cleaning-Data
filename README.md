This file describes how run_analysis.R script works.

1.First,download and unzip the data file called "UCU HAR Dataset.zip"
2.Make sure your working directory has been set correctly. Also, the unzipped file has to be in
  the working directory for the code to work. You can change the working directory by changing 
  the location via the code "setwd()"

3.Second, use source("run_analysis.R") command in R
4.You will find two output files are generated in the current working directory:
  "merged_Alldata.txt"
  "MeanSD_Tidy_Data.txt"

5. Finally, use data <- read.table("MeanSD_Tidy_Data.txt") command in R to read the file. 
   When performing the dim() function on MeanSD, you should find 180 rows and 68 columns
