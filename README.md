# Prepping data 4 R 

An R MeetUP to explore prepping data for analyses in R.

### Project Overview

We will be using Callie and Laura's project as an example of dealing with real data. Here is a quick overview of their project:

Part of their group project at the Bren School is creating a marine spatial plan that identifies ideal vessel traffic routes that avoid hotspots of sperm whale activity to reduce whale-vessel strikes. To do this, we need to take multiple datasets and combine them with common characteristics to create one large database. 

Our goal is to enable easy data input and update for future analyses. 

### Data sets

The datasets we have included here are: 

1. Research vessel tracks (time, lat, long)
2. Whale clusters (DateTime)
3. AIS vessel data (lat, long)

### Challenges

- The whale clusters dataframe includes time stamps of sperm whale sightings off the west coast of Dominica. However, there are no GPS coordinates associated with those sightings. Since the research vessel tracks dataframe does have GPS coordinates associated with it, we need to match up the corresponding date/time of the whale sightings with the location the research vessel was at when it made those sightings. This will give us coordinates of whale sightings so that we can map species presence off the west coast of Dominica.

- The second step is to compile all our separate AIS dataframes into one in order to map current vessel activity off the west coast of Dominica and eventually overlay that with the sperm whale species presence data.
