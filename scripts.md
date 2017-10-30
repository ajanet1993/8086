## Set working directory
setwd("D:/college/cs8086_data2decisions/Project")

## Read csv file
ghg1<-read.csv("air-n-ghg.csv",header=TRUE,stringsAsFactors=FALSE)

## Convert strings to factors
### converting Subject into factors
ghg1$SUBJECT <- factor(ghg1$SUBJECT)

### converting Region into factors
ghg1$Region <- factor(ghg1$Region)

### converting measure into factors
ghg1$MEASURE <- factor(ghg1$MEASURE)

## View a summary of data
summary(ghg1)

## creating a subset for CO2 
ghg.sub <- ghg1[ghg1$SUBJECT == 'CO2', ]

## creating a subset for CO2 measured in Millions of Tons
ghg.sub2 <- ghg.sub[ghg.sub$MEASURE == 'MLN_TONNE', ]

## creating a subset for CO2 for time 2000-2014
ghg.sub3 <- ghg.sub2[ghg.sub2$TIME>2000 & ghg.sub2$TIME<2015, ]

## Scatterplot between time and value
plot(ghg.sub3$Value~ghg.sub3$TIME)

## Scatterplot between region and value
This plot explains about the CO2 emission content based on region.
plot(ghg.sub3$Value~ghg.sub3$Region)

## creating a subset of CO2 values for year 2012.
ghg.sub2012<-ghg.sub3[ghg.sub3$TIME==2012,]

## Rank in descending order based on most Urbanized regions from 2012,top 20:
top52012 <- head(ghg.sub2012[order(ghg.sub2012$Urbanization., decreasing= T),], n = 15,)

## Create a barchart of Top Urbanizied Regions 2012:
barplot(top52012$Urabnization., main="Top Urbanizied Regions 2012", col = rainbow(20), space=0)
axis(1, at=.5:19.5, labels=top2014$region)

