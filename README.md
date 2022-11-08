# MACAD THESIS - UNRAVELLING THE SEASONAL CITY - IN PROGRESS
This app allows to discover alternative pedestrian paths in the city. By defining a Start Point (A) and an End Point (B), the user can explore the most attractive route each month in terms of seasonality of the urban forest.

## STATE OF THE ART
## COMMON ISSUES
The tree layer has been uploaded directly on Mapbox using Mapbox Studio. It should be updated and upload from the script itself.

## INDEX 01
The Shortest Path is visible thanks to the Mapbox Directions API (should come from the Python file), but only by fixing a static Start Point. By entering an address (which could also be interesting as Start Point), a marker is created, but the route still appears between the fixed static Start Point and the clicked dinamic End Point.

## INDEX 02
By modifying the map on.click function, both Start and End Points should be created by clicking on the map, but the code resets itself with each click, continuosly creating the Start Point and not allowing to set the End Point.

## INDEX 03
A path can be drawn and it is converted to the Shortest Path thanks to the Mapbox Directions API, but it only works with a minimum of 3 points instead of 2, and it generates an error if the distance between points is larger than 50m (now set as 25). Also, the web must be reload to start a new route.

## INDEX 04
A Start and End Points can be defined by the user. To avoid INDEX 02 issue, the Start is defined by Double Clicking (blue dot) and the End by Single Clicking (pink dot). The Mapbox Direction API does not create the shortest route (no idea why), although this should not be a problem as the route should be calculated by the python file. Also, a time slider with the months has been built (the earthquake geojson should be updated with the Tree geojson).

## Credits
UNRAVELLING THE SEASONAL CITY is a project of IAAC, Institute of Advanced Architecture of Catalonia developed at MaCAD, Master In Advanced Computation For Architecture & Design in 2021/2022 by Student: Lucía Leva Fuentes, and Thesis Advisor: David Andres León.