# Houston power outages February 2021

An assignment for EDS223: Geospatial Analysis and Remote Sensing for the Masters of Environmental Data Science Program at UCSB.

The goal of the project is to gain experience working with large spatial data in R by using remotely sensed night light data, highway, housing, and income data to look at the relationship between homes in Houston, Texas that lost power during the February 2021 storms and median income census tract. Analysis steps include:

1. Reading in data files using the `stars` package
2. Preparing the raster data for manipulation
3. Excluding highway lights from data
4. Estimating the number of homes that lost power
5. Mapping the census tracts that lost power and their median income

## Citations
Data was obtained from:

[OpenStreetMap](https://www.openstreetmap.org/#map=4/38.01/-95.84)

[US Census Bureau](https://data.census.gov/)

[Visible Infrared Imaging Radiometer Suite (VIIRS)](https://en.wikipedia.org/wiki/Visible_Infrared_Imaging_Radiometer_Suite)

## File Structure

    houston-poweroutages
    │   README.md
    |   .gitignore
    │   houston-power-outages.qmd    
    │
    └───data
        |   gis_osm_roads_free_1.gpkg
        |   gis_osm_buildings_a_free_1.gpkg
        |
        └───VNP46A1
        │   │   night light .tif files 
        |
        └───ACS_2019_5YR_TRACT_48_TEXAS.gdb
        |   │   Texas census geometries

