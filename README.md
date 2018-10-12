# Microsoft_codefundo-_2018

## Flood Prediction
To predict floods, we need a parallel data flow in the real time from the following sources:
1)	Meteorological unit (weather forecasting)
2)	Hydrological unit (climate changes in water resources, Hydraulic Modelling)
3)	Past data of floods of a given region

## Process Overview:
### 1)	Data Processing: 
  1.	Rainfall forecast data is collected every 10-15 minutes 
  2.	Water resources of different water bodies near the Region X are identified and their water levels data is collected from the Hydrological department.
  3.	Data from different external sources can also be channeled into the system depending on the situation involved.
  4.	We will resolve the high level of inconsistency in the incoming data so that the flood prediction module can work efficiently to give greater accuracy.


### 2)	Forecasting: 
  1.	Mathematical models that convert data, such as rainfall measured by either rain gauges or radars, into river discharge for a further assessment of the forthcoming flooding is done here.
  2.	Let say there is a point P located on the map where we need to forecast the weather. We first find the nearest points near the point P where the rain gauges are installed and the water levels of those points are collected. (x1,x2,x3,….xN)
  3.	Weighted-average (based on distance from the point P) is used to interpolate to initially forecast water level at point P.
  4.	Finally, the effect from the data collected from the other external sources is added.
  5.	(i.e Is the area in a high-risk zone? Is it a low-lying area? Any recent geographical or climatic change?) and then an expected water level in the given region X is generated.

### 3)	Information Channeling:
  1.	If the critical predicted water level of the region X is found to be greater than the critical water level, the warnings can be forwarded to the decision makers in the real time.
  2.	These decision makers can then analyze the conditions and then can direct the Flood Relief teams, pumps, etc. to be dispatched.
  3.	Another methodology – “Evacuation Optimization” can be used to assist the teams as to where in they should set up their relief camps. In this, factors like geographical terrain & natural habitat can be considered. <br>

Let’s say we live in city X , the reasons which can cause flood in the city can be varying , but the major reasons are listed as follows –
  1.	Regardless of the rains the problems are: dams and overbuilding. Typically the rain water is absorbed by the ground. Cities are all cemented and paved and the whole water of a large area is channelled into drains and poured into rivers raising their level.
  2.	Global warming , As average temperatures in regions across the country(India) have gone up, more rain has fallen during the heaviest downpours. This happens because warmer air holds more moisture. This fact is apparent when you see water vapor hanging in the air after turning off a hot shower. When warm air holding moisture meets cooler air, the moisture condenses into tiny droplets that float in the air. This leads to heavy precipitation and flooding .

