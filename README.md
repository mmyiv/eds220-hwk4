# Visualizing 2017 Thomas Fire Scars
## Author: [Michelle Yiv](https://github.com/mmyiv)

# Purpose

This repository contains 2 Jupyter notebooks of the Thomas Fire boundary, and visualization and analysis of that fire near Santa Barbara

# Repository Structure

eds220-hwk4
│   README.md
|   hwk4-task2-fire-perimeter-YIV.ipynb
│   hwk4-task2-false-color-YIV.ipynb
|   .gitignore
│
└───data
    │ California_Fire_Perimeters_(all).cpg
    │ California_Fire_Perimeters_(all).dbf
    │ California_Fire_Perimeters_(all).prj
    │ California_Fire_Perimeters_(all).shp.xml
    │ California_Fire_Perimeters_(all).shx
    │ thomas_fire.cpg
    │ thomas_fire.dbf
    │ thomas_fire.prj
    │ thomas_fire.shp
    │ thomas_fire.shx

# Data Access
Thomas Fire Boundary data can be downloaded through the Data.gov, and is housed on the Bren Workbench Server. Data can be read in through the `GeoPandas` package. Data was filtered to the Thomas 2017 Fire and was plotted as a boundary.

Landsat data was sourced by the EDS 220 Instructor and is housed on the Bren Workbench server. It was sourced from the Microsof Planetary Computer data catalogue and was cleaned beforehand to remove land data outside of Santa Barbara and to coarsen resolution.  To run the code, data is read in using `xarray` and `rioxarray` packages. Coordinates refer to the area surrounding Santa Barbara, and data variables are used to plot true/false color images.


# References

EDS 220 - Working with Environmental Datasets Course Notes.
Date of Access: 11-19-2024.
[Link to data]([https://meds-eds-220.github.io/MEDS-eds-220-course/book/preface.html](https://meds-eds-220.github.io/MEDS-eds-220-course/book/chapters/lesson-15-rioxarray/lesson-15-rioxarray.html)
Citation: "EDS 220 - Working with Environmental Datasets Course Notes," EDS 220 - Working with Environmental Datasets Course Notes. 2024. EDS 220 - Working with Environmental Datasets Course Notes. (accessed Nov. 19, 2024).

California Fire Perimeter.
Date of access: 11-19-2024.
[Link to data](https://catalog.data.gov/dataset/california-fire-perimeters-all-b3436)
Citation: “Data.gov,” Data.gov, 2024. https://catalog.data.gov/dataset/california-fire-perimeters-all-b3436 (accessed Nov. 19, 2024).

Landsat Data.
Date of access: 11-19-2024.
[Link to data](https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2)
Citation: “Microsoft Planetary Computer,” Microsoft.com, 2024. https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2 (accessed Nov. 19, 2024).


    
    
    
