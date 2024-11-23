# Fire Scars from the 2017 Thomas Fire in Santa Barbara and Ventura

## About 
This repository is part of an assignment for the class EDS-220 Environmental Datasets at University of California, Santa Barbara as part of the Master's of Environmental Data Science program with the Bren School for Environmental Science and Management.


<figure>
<p align="center">
<img 
  src="/images/helicopter.jpg" 
  width="800"
  >
  <figcaption>Helicopter prepare's to put out a wildfire in California.
  </figcaption>
</p>
</figure>

## Description

### Explanation
- `hwk4-task2-fire-perimeter-COHEN.ipynb` contains code for loading, cleaning, and subsetting the historical fire perimeter data (`California_Fire_Perimeters_(1950%2B)`) for the 2017 Thomas Fire boundary.
- `hwk4-task2-false-color-COHEN.ipynb` contains code for loading, cleaning, and plotting the landsat data array (`landsat8-2018-01-26-sb-simplified`). A false color raster is created from NIR and SWIR bands as well as the Thomas Fire boundary overlaid on top to highlight the resulting fire scar.
- `data/`
    - `California_Fire_Perimeters_(1950+)` is a shapefile containing more than 15000 records of CA fire perimeter data through 1898 to 2023.
    - `thomas_perim` is a subset of the CA fire perimeters shapefile containing a single row for the 2017 Thomas Fire.
    - `landsat8-2018-01-26-sb-simplified` is a data array from remote sensing satellite Landsat, from Landsat Collection 2 Level-2. It is pre-processed with reduced resolution and an extent centered around Santa Barbara. It contains 1 band, 3 dimensions, 3 visible light variables, and 2 infrared variables.

### File Organization
```
eds220-hwk4
│
├── README.md                     
├── hwk4-task2-fire-perimeter-COHEN.ipynb  # .ipynb for subsetting Thomas 2017
├── hwk4-task2-false-color-COHEN.ipynb  # .ipynb for plotting
│
├── data/
│   ├── California_Fire_Perimeters_(1950+)
│      ├── California_Fire_Perimeters_(1950%2B).shp
│   ├── thomas_perim
│   ├── landsat8-2018-01-26-sb-simplified
│
├── images/                       
│   ├── helicopter.jpg             # Image used in the README
│
├── .gitignore 
```

## Data Access

The data needed for this analysis is not stored in the repository. The datasets can be down loaded from their respective databases.

- `California_Fire_Perimeters_(1950+)` can be downloaded from [California Natural Resources agency](https://gis.data.cnra.ca.gov/datasets/CALFIRE-Forestry::california-fire-perimeters-1950-1/explore) website.
- `landsat8-2018-01-26-sb-simplified` is a pre-processed file and the only way to access it is through University of California, Santa Barbara's Posit Workbench server. However, a similar Landsat image of Santa Barbara can be downloaded from the [Microsoft Planetary Computer](https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2) data catalogue.

## Acklowledgements

### This project is supported in part by:
- EDS 220 Environmental Datasets at UCSB: [Website](https://meds-eds-220.github.io/MEDS-eds-220-course/)
- UCSB Bren School for Environmental Science and Management: [Website](https://bren.ucsb.edu/)
- The Master of Environmental Data Science degree at Bren: [Website](https://bren.ucsb.edu/masters-programs/master-environmental-data-science)
- National Center for Ecological Analysis and Synthesis (NCEAS): [Website](https://www.nceas.ucsb.edu/)
- Sam Csik: [Website](https://samanthacsik.github.io/)

### Data Citations

Earth Resources Observation and Science (EROS) Center. (2020). Landsat 8-9 Operational Land Imager / Thermal Infrared Sensor Level-2, Collection 2 [dataset]. U.S. Geological Survey. [link](https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2)

California Department of Forestry and Fire Protection (2024), California Historical Fire Perimeters [dataset]. California Natural Resources Agency.[link](https://gis.data.cnra.ca.gov/maps/CALFIRE-Forestry::california-historical-fire-perimeters/about)