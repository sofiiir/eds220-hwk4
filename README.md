# EDS220: Visualizing Palisades and Eaton Fire Scars through False Color
#### Author: Sofia Rodas

This repository fulfills homework 4 for the course 220: Working with Environmental Data Sets as part of the Masters of Environmental Data Science program through the Bren School of Environmental Science and Management at the University of California Santa Barbara. 

<img width="645" height="390" alt="Screenshot 2025-11-23 at 6 48 27 PM" src="https://github.com/user-attachments/assets/722a1049-bb44-4aa9-9f87-2f32a218d500" />


Final false color imagery map depicting the Eaton and Palisades Fires.

## About

**1. Purpose:** 
- This repository maps NASA and USGS Landsat8 data and National Interagency Fire Center (NIFC) fire boundaries data depicting the Eaton and Palisades Fires that occured in January of 2025. The final result is a false color map showing clear colorations of the fire scars with an overlay of the official fire boundaries. 

**2.  Highlights:** 
- Landsat data is read in with NetCDF. No CRS is originally assigned to the entire Landsat data. The CRS is held in the `spatial_ref` variable. The GeoSpatial data must be restored by using the CRS from the `spatial_ref` variable. 

- Landsat data is versatile. Landsat 8 has 11 bands that can be selected to make a variety of coloration maps. For example, the red, green, and blue bands (in that order) can be selected in that order to create a true coloration map. 

- False color Landsat maps are created by selecting the short-wave infrared (swir22), near-infrared, and red variables (in that order). This map best depicts the fire scars on the landscape. The final map shows the fire scars with the additional boundaries of the fires being included for clarity. 

**3. Datasets descriptions:** 
- **Eaton and Palisades Fire perimeters:** The fire perimeter data was acquired from the City of Los Angeles official GeoHub. This City of Los Angeles GIS data is originally from the National Interagency Fire Center (NIFC) through the Fire Integrated Real-time Intelligence System (FIRIS). Eaton fire and Palisades fire perimeters are included in this download. This data is publicly available.

- **Landsat8:** NASA Landsat satellites in conjunction with USGS acquire data using 11 bands through the use of Operational Land Imager (OLI) and the Thermal Infrared Sensor (TIRS). Landsat satellites orbit earth at a rate of 16 days per cycle making imaging availability satelite location dependent. This data is publicly available.


## Data Access:

- **Data download:**

  1. The Landsat8 data was downloaded from the courses data Google Drive that can be accessed [here](https://drive.google.com/drive/folders/1USqhiMLyN8GE05B8WJmHabviJGnmAsLP). Landsat8 data can also be downloaded through the USGS webpage at [https://earthexplorer.usgs.gov/](https://earthexplorer.usgs.gov/). This data is publicly available.

  2. Eaton and Palisades Fire boundary data was downloaded from the City of Los Angeles ArcGIS hub. It can be accessed at [https://geohub.lacity.org/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about](https://geohub.lacity.org/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about). This data is publicly available.


## Repository structure: 

<img width="442" height="97" alt="Screenshot 2025-11-23 at 6 43 41 PM" src="https://github.com/user-attachments/assets/b33968be-2fe7-4b64-97cf-0260e4ba105d" />

Note: The data files were added to the .gitignore. See data access above for details on data acquisition.

## References:

- C. Galaz Garcia and A. Adams, EDS 220 - Working with Environmental Datasets. (n.d.) Available: https://meds-eds-220.github.io/MEDS-eds-220-course/. [Accessed November 17, 2025]

- City of Los Angeles GeoHub / NIFC FIRIS(2025).Palisades and Eaton Dissolved Fire Perimeters (2025) [Shapefile]. Available: https://egis-lacounty.hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about. [Retrieved November 17, 2025]
  
- Earth Resources Observation and Science (EROS) Center. (2020). Landsat 8-9 Operational Land Imager / Thermal Infrared Sensor Level-2, Collection 2 [dataset]. U.S. Geological Survey. https://doi.org/10.5066/P9OGBGM6. Available: https://www.usgs.gov/centers/eros/science/usgs-eros-archive-landsat-archives-landsat-8-9-olitirs-collection-2-level-2. [Accessed November 17 ,2025]

- NASA Earth Observatory. (2014, Mar. 4). Why is that forest red and that cloud blue? How to interpret a false-color satellite image_. Available: https://earthobservatory.nasa.gov/features/FalseColor.
[Accessed: Nov. 18, 2025]

- U.S. Geological Survey. (n.d.). What are the band designations for the Landsat satellites?_ Available: https://www.usgs.gov/faqs/what-are-band-designations-landsat-satellites. [Accessed: Nov. 18, 2025]

- U.S. Geological Survey. (2021, Nov. 12). _Common Landsat band combinations_. Available: https://www.usgs.gov/media/images/common-landsat-band-combinations. [Accessed: Nov. 18, 2025]
