# Project - Data Entry Analysis
## Author - Anuja Janet

## List of files in the Directory

1. pond2010.xlsx
2. zoop-temp.xlsx
3. zoop-temp-main.xlsx
4. Data Entry Analysis.md

## Background
Plankton are microscopic organisms that form the base of many aquatic food webs – fueling the growth of fish and other larger organisms. It’s common to sample them using a net or another container that can be controlled to collect water just from certain depths; so you can see how plankton collected at the surface (0 meters) might be different from plankton at another depth (e.g. 10 meters below the surface).
They are identified and counted under a microscope, and usually their numbers are reported as individuals per liter or milliliter.

Frequently, aquatic scientists collect plankton samples during both day (e.g. noon) and night (e.g. 2 am) because plankton change their distributions from day to night, and not all species alter their distributions in the same way. (For more information, search “diel vertical migration” on the web.)
The 3 files linked above were all intended to be part of the same study – the investigators wanted to examine the day-night distribution of 2 species of zooplankton across multiple years. The type of zooplankton they studied is called rotifers generally, and specifically the genus Conochilus, in which groups of individual rotifers stick together in colonies (see http://eol.org/pages/43393/overview (Links to an external site.)Links to an external site.). The investigators plan to repeat this study for several more years.

## Problems with the Given Data
1.	Year Difference – Pond2010 file has data related to Rotifer’s species namely Cuni and Chippo for the year 2010, where as the 		other files, zoop-temp and zoop-temp-main has data collected for year 2011.
2.	Pond2010 has a column ‘z’ which is undefined.
3.	Station A and Station B terms are not clearly explained. 
4.	Column metrics are not mentioned.
5.	Missing column values for certain rows.
6.	Yellow notebook for map and details has no clear explanation.
7.	Chippo #/L has few negative values which is impossible.
8.	Unconventional values of the specimen are presented which does not support the fact of co-existence.
9.	Does not provide the basic information to examine the day-night distribution of species i.e., data related to time.
10.	The file zoop-temp-main consists data for 3 dates 06/04, 06/07, 06/09 compared to the file zoop-temp which has data 
	for 2 dates 06/07, 06/09.
11.	Temperature column in zoop-temp-main has one large outlier.

## Response to the above stated problems.
The issues that are stated can be resolved as follows.
1. The data in all 3 files can be combined into one file.
2. New column 'time' should be added to get information related to day and night distribution of species.
3. Each column should be clearly stated with units of measurement.
4. Combining all 3 files into one file makes the data analysis task easy and efficient.

## Potential Table that can address the issues.

| Date (MM/DD/YY) | Time (HH:MM:SS) | Species | Colony Diameter (mm) | Depth(m) | Temperature(celsius) | Cuni #/L | Cuni ColonySize(mm) | Chippo #/L | Chippo ColonySize(mm) | Chla | Station |
|-----------------|-----------------|---------|----------------------|----------|----------------------|----------|---------------------|------------|-----------------------|------|---------|

Table consists of 12 columns. 

### This table is useful to examine the day-night distribution of 2 species of zooplankton across multiple years.
1. Date and time columns are used to examine the data across multiple years for a particular time.
2. The other columns are used to analyze the behaviour and distribution of cuni and chippi species.
3. Time column is a new column which fulfills the criteria of day-night distribution.
4. Each column is represented with unit of measurement to avoid confusion about units.
5. The values in each columns should be without outliers.

