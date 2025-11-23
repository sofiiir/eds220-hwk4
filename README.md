# EDS220: Visualizing Palisades and Eaton Fire Scars through False Color
#### Author: Sofia Rodas

This repository fulfills homework 4 for the course 220: Working with Environmental Data Sets as part of the Masters of Environmental Data Science program through the Bren School of Environmental Science and Management at the University of California Santa Barbara. 

<img width="649" height="392" alt="Screenshot 2025-11-23 at 3 31 13 PM" src="https://github.com/user-attachments/assets/22d0b883-d670-403a-8bd9-daaf38d8e09d" />


## About

**1. Purpose:** 
- This repository explores maps NASA and USGS Landsat8 data and National Interagency Fire Center (NIFC) fire boundaries data depicting the Eaton and Palisades Fires that occured in January of 2025. The final result is a false color map showing clear colorations of the fore scars with an overlay of the official fire boundaries. 

**2.  Highlights:** 
- Landsat data is read in with NetCDF. No CRS is originally assigned to the entire Landsat data. The CRS is held in the `spatial_ref` variable. The GeoSpatial data must be restored by using the CRS from the `spatial_ref` variable. 

- Landsat data is versatile. Landsat 8 has 8 bands that can be selected to make a variety of coloration maps. For example, the red, green, and blue bands (in that order) can be selected in that order to create a true coloration map. 

- False color Landsat maps are created by selecting the short-wave infrared (swir22), near-infrared, and red variables (in that order). This map best depicts the fire scars on the landscape. The final map shows the fire scars with the additional boundaries of the fires being included for clarity. 

**3. Datasets descriptions:** 
- Eaton Fire perimeter: The fire perimeter data was acquired from the Los Angeles County official GIS catalogue. This Los Angeles County GIS data is originally from the National Interagency Fire Center (NIFC) through the Fire Integrated Real-time Intelligence System (FIRIS). It contains the boundary of the Eaton Fire.

- Palisades Fire perimeter: The fire perimeter data was acquired from the Los Angeles County official GIS catalogue. This Los Angeles County GIS data is originally from the National Interagency Fire Center (NIFC) through the Fire Integrated Real-time Intelligence System (FIRIS). It contains the boundary of the Palisades Fire.

- Landsat8: NASA Landsat satellites in conjunction with USGS acquire data using 11 bands through the use of Operational Land Imager (OLI) and the Thermal Infrared Sensor (TIRS). Landsat satellites orbit earth at a rate of 16 days per cycle.


## Data Access:

- **Data download:**

  1. The Landsat8 data was downloaded from the courses data Google Drive that can be accessed [here](https://drive.google.com/drive/folders/1USqhiMLyN8GE05B8WJmHabviJGnmAsLP). Landsat8 data can also be downloaded through the USGS webpage at [https://earthexplorer.usgs.gov/](https://earthexplorer.usgs.gov/)

  2. Eaton and Palisades Fire boundary data was downloaded from the City of Los Angeles ArcGIS hub. It can be accessed at [https://geohub.lacity.org/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about](https://geohub.lacity.org/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about) .


## Repository structure: 

<img width="399" height="100" alt="eds220-hwk4-tree" src="https://github.com/user-attachments/assets/821875e2-6870-476c-9b66-b856948ee881" />

Note: The data files were added to the gitignore. See data access above for details on data acquisition.

## References:

- Earth Resources Observation and Science (EROS) Center. (2020). Landsat 8-9 Operational Land Imager / Thermal Infrared Sensor Level-2, Collection 2 [dataset]. U.S. Geological Survey. https://doi.org/10.5066/P9OGBGM6. Available: [Accessed November 17 ,2025]

- City of Los Angeles GeoHub / NIFC FIRIS(2025).Palisades and Eaton Dissolved Fire Perimeters (2025) [Shapefile]. Available: https://egis-lacounty.hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about. [Retrieved November 17, 2025]

