# Visualizing 2017 Thomas Fire Scars
## Author: [Michelle Yiv](https://github.com/mmyiv)

![Thomas Fire, December 2017. Source: https://sbbucketbrigade.org/timeline/2017-thomas-fire/](https://github.com/user-attachments/assets/ef34594a-a22b-4e85-be88-0c7448303de4)

# Purpose
The Thomas Burned 281,000 acres in Santa Barbara and Ventura County from December 4th to January 12, 2018. Analysis of this fire is contained in this repository. Landsat and CalFire boundary data were used to map the burn scars with true and false color imagery, and Air Quality Index data from the US EPA was analyzed to visualize the impacts of air quality over time from the fire.

# Repository Structure
```
eds220-hwk4
│  └──README.md
|  └──hwk4-task2-fire-perimeter-YIV.ipynb
│  └──hwk4-task2-false-color-YIV.ipynb
|  └──blogpost_yiv.ipynb
|  └──.gitignore
│
└───data
    │ └──California_Fire_Perimeters_(all).cpg
    │ └──California_Fire_Perimeters_(all).dbf
    │ └──California_Fire_Perimeters_(all).prj
    │ └──California_Fire_Perimeters_(all).shp.xml
    │ California_Fire_Perimeters_(all).shx
    │ └──thomas_fire.cpg
    │ └──thomas_fire.dbf
    │ └──thomas_fire.prj
    │ └──thomas_fire.shp
    │ └──thomas_fire.shx
```
# Data Access
Thomas Fire Boundary data can be downloaded through the Data.gov, and is housed on the Bren Workbench Server. Data can be read in through the `GeoPandas` package. Data was filtered to the Thomas 2017 Fire and was plotted as a boundary.

Landsat data was sourced by the EDS 220 Instructor and is housed on the Bren Workbench server. It was sourced from the Microsof Planetary Computer data catalogue and was cleaned beforehand to remove land data outside of Santa Barbara and to coarsen resolution.  To run the code, data is read in using `xarray` and `rioxarray` packages. Coordinates refer to the area surrounding Santa Barbara, and data variables are used to plot true/false color images.

Air quality data was sourced by the US Environmental Protection Agency, and contain information about AQI values by county from 2017 and 2018. Data can be read in using the `pandas` package. Data was concatenated to combine AQI information of all 2017 for the Thomas Fire. Data was cleaned and made tidy to compute a rolling average and plot AQI values.


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

Air Quality Index Data
Date of Access: 10-29-2024
[Link to data](https://www.airnow.gov/aqi/aqi-basics/)
Citation: "AQI Basics," airnow.gov, 2021. https://www.airnow.gov/aqi/aqi-basics/ (accesed Oct. 29, 2024)

Thomas Fire Photo and Statistics
Date of Access: 12-04-2024
[Link to website](https://sbbucketbrigade.org/timeline/2017-thomas-fire/)
Citation: "2017 Thomas Fire," sbbucketbrigade. 2019. https://sbbucketbrigade.org/timeline/2017-thomas-fire/
    
    
    
