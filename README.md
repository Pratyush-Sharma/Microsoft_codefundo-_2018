# Microsoft_codefundo-_2018

## Flood Prediction
Suppose we need to predict the floods in a region X. To predict floods, we need a parallel data flow in the real time from the following sources:
1)	Meteorological unit (weather forecasting)
2)	Hydrological unit (climate changes in water resources, Hydraulic Modelling)
3)	Past data of floods of a given region

## Process Overview:
### 1)	Data Processing: 
  1.	Rainfall forecast data is collected every 10-15 minutes 
  2.	Water resources of different water bodies near the Region X are identified and their water levels data is collected from the Hydrological department.
  3.	Data from different external sources can also be channeled into the system depending on the situation involved.
  4.	There will be high level of inconsistency in the incoming data from different sources. We will resolve these inconsistency so that the flood prediction module can work efficiently to give greater accuracy.

### 2)	Forecasting: 
  1.	Mathematical models that convert data, such as rainfall measured by either rain gauges or radars, into river discharge for a further assessment of the forthcoming flooding is done here.
  2.	Let say there is a point P located on the map where we need to forecast the weather. We first find the nearest points near the point P where the rain gauges are installed and the water levels of those points are collected. (x1,x2,x3,….xN)
  3.	Weighted-average (based on distance from the point P) is used to interpolate to initially forecast water level at point P.
  4.  This initial forecast is refined by adding on the impact/effect that can be caused due to the changes in water levels near the point P. (Data coming from the Hydrological unit)
  5.	Finally, the effect from the data collected from the other external sources is added (i.e Is the area in a high-risk zone? Is it a low-lying area? Any recent geographical or climatic change?) 
  6. Finally, an 'expected water level' in the given region X is generated. (Monte Carlo method)

### 3)	Information Channeling:
  1. We collect the historical data of the given place and evaluate the 'critical water levels' that has caused the floods in the region previously.
  2.	If the 'predicted water level' of the region X is found to be greater than the 'critical water level', the warnings can be forwarded to the decision makers in the real time.
  3.	These decision makers can then analyze the conditions and then can direct the Flood Relief teams, pumps, etc. to be dispatched.
  4.	To further help them “Evacuation Optimization” can be used to assist the teams as to where in they should set up their relief camps. In this, the places in the geographical map are chosen such that it is
          i)   Closer to the flood affected areas
          ii)  Closer to the dispatch teams
          iii) Is safe
