# EDS220: Visualizing Palisades and Eaton Fire Scars through False Color
#### Author: Sofia Rodas

## About

**1. Purpose:** 
- This repository explores maps NASA and USGS Landsat8 data and National Interagency Fire Center (NIFC) fire boundaries data depicting the Eaton and Palisades Fires that occured in January of 2025. The final result is a false color map showing clear colorations of the fore scars with an overlay of the official fire boundaries. 

**2.  Highlights:** 
- Landsat data is read in with NetCDF. No CRS is originally assigned to the entire Landsat data. The CRS is held in the `spatial_ref` variable. The GeoSpatial data must be restored by using the CRS from the `spatial_ref` variable. 

- Landsat data is versatile. Landsat 8 has 8 bands that can be selected to make a variety of coloration maps. For example, the red, green, and blue bands (in that order) can be selected in that order to create a true coloration map. 

- False color Landsat maps are created by selecting the short-wave infrared (swir22), near-infrared, and red variables (in that order). This map best depicts the fire scars on the landscape. The final map shows the fire scars with the additional boundaries of the fires being included for clarity. 

**3. Datasets description:** 
- Eaton Fire perimeter: The fire perimeter data was acquired from the Los Angeles County official GIS catalogue. This Los Angeles County GIS data is originally from the National Interagency Fire Center (NIFC) through the Fire Integrated Real-time Intelligence System (FIRIS). It contains the boundary of the Eaton Fire.

- Palisades Fire perimeter: The fire perimeter data was acquired from the Los Angeles County official GIS catalogue. This Los Angeles County GIS data is originally from the National Interagency Fire Center (NIFC) through the Fire Integrated Real-time Intelligence System (FIRIS). It contains the boundary of the Palisades Fire.

- Landsat8: NASA Landsat satellites in conjunction with USGS acquire data using 11 bands through the use of Operational Land Imager (OLI) and the Thermal Infrared Sensor (TIRS). Landsat satellites orbit earth at a rate of 16 days per cycle.


## Data Access:

-**Data download:** 


## File structure:

## Repository Contents:

## References:

- Earth Resources Observation and Science (EROS) Center. (2020). Landsat 8-9 Operational Land Imager / Thermal Infrared Sensor Level-2, Collection 2 [dataset]. U.S. Geological Survey. https://doi.org/10.5066/P9OGBGM6 [Accessed November 17 ,2025]

- NIFC FIRIS(2025).Palisades and Eaton Dissolved Fire Perimeters (2025) [Shapefile]. County of Los Angeles. https://egis-lacounty.hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about. [Retrieved November 17, 2025]

### References:
[Palisades and Eaton Dissolved Fire Perimeters](https://egis-lacounty.hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about)
