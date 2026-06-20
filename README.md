# Cooling Off on the Danube

An interactive web map and enriched dataset of pontoons and recreational spots on Vienna’s Donauinsel.

## Project Overview

**Cooling Off on the Danube** is a web map and dataset about pontoons on Vienna’s Donauinsel. The aim of the project is to make it easier to choose suitable chill and resting spots on the island, one of Vienna’s most important recreational areas during hot summer days.

The project provides both:

* an interactive Leaflet web map for exploring pontoon locations
* an enriched dataset that can be reused for spatial analysis, visualization, or further research.

The original open data was extended with project-specific information such as shade availability, lawn condition, chill area, nudism area information, distances to nearby infrastructure and pictures.

## Web Map

Check out the interactive map here:

**[Cooling Off on the Danube](https://wiwi1999.github.io/danube-pontoon-map/)**

The map includes:

* interactive markers for pontoon locations
* popups with detailed information and photos
* filters for shade, lawn availability, nudism area information, and minimum chill area
* multiple basemaps, including OpenStreetMap, Carto Light, and ESRI Satellite
* a feedback button for suggesting updates or corrections

## Data Sources and Attribution

This project uses and extends open data from the City of Vienna and ÖVDAT/GIP.at.

The base dataset is “Donauinsel Freizeiteinrichtungen Standorte Wien” by Stadt Wien, published via data.gv.at. GIP / Graphenintegrations-Plattform Österreich data by ÖVDAT, published via data.gv.at,  was used for spatial analysis and network-based distance calculations.

Attribution:

* Stadt Wien - data.wien.gv.at
* ÖVDAT/GIP.at - Graphenintegrations-Plattform Österreich

Full source citations, license information, and attribution requirements are provided in the metadata and license files.

## Data Collection and Network Analysis

The final dataset combines:

* official open data from the City of Vienna
* field-collected observations
* manually added photos
* network analysis based on ÖVDAT data

Field observations were collected on the following dates: `06.,09.,13. June 2026`. They include information about:

* shade availability
* lawn or ground condition
* estimated chill or resting area
* nudism area information
* pictures

Network analysis was used to calculate approximate distances to nearby infrastructure such as first aid stations and restaurants or bistros. These distances should be used for orientation only.

## Dataset Attributes

| Attribute     | Type                     | Description                                                                                                                     |
| ------------- | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------- |
| `ORTBESCHR`   | Text                     | Original location description from the source dataset.                                                                          |
| `CHILL_AREA`  | Number                   | Estimated available chill or resting area in square meters.                                                                     |
| `SHADE`       | Boolean coded as integer | Shade availability. `0` = no shade, `1` = shade available.                                                                      |
| `LAWN`        | Categorical integer      | Lawn or ground condition recorded during field collection. `1` = mowed, `2` = medium height, `3` = high grass, `4` = sand/soil. |
| `c_lat`       | Number                   | Latitude coordinate used for map display.                                                                                       |
| `c_lon`       | Number                   | Longitude coordinate used for map display.                                                                                      |
| `lawn_date`   | Date                     | Date when the lawn or ground condition was recorded.                                                                            |
| `lawn_text`   | Text                     | Text version of the lawn or ground condition category, for example “mowed”, “medium height”, “high grass”, or “sand/soil”.      |
| `nudism_area` | Text                     | Indicates whether the location is within a nudism area.                                                                         |
| `dist_first`  | Number                   | Approximate network-based distance to the nearest first aid station, measured in meters.                                        |
| `dist_food`   | Number                   | Approximate network-based distance to the nearest restaurant or bistro, measured in meters.                                     |

## Usage

The dataset can be used to:

* explore recreational infrastructure on the Donauinsel,
* compare pontoon locations based on shade, lawn condition, and available chill area,
* identify nearby food or first aid infrastructure,
* support further spatial or network-based analysis,
* update or improve the interactive web map.

## Limitations

Some information is based on observation or estimation and may change over time. Distances are approximate and should be used for orientation only. Shade availability can vary depending on the time of day, season, weather, and surrounding vegetation.

## Feedback and Contributions

The map includes a GitHub issue button that allows users to License and Attribution
The original datasets are licensed under Creative Commons Attribution 4.0 International — CC BY 4.0.

License text: https://creativecommons.org/licenses/by/4.0/

Attribution for the City of Vienna dataset:

Stadt Wien – data.wien.gv.at

Attribution for the GIP dataset:

ÖVDAT/GIP.at – Graphenintegrations-Plattform Österreich

This derived dataset includes changes to the original data. It was enriched with field-collected observations, additional attributes, photos, and spatial analysis results.

Users of this dataset must credit this derived dataset as well as the original data sources listed above.suggest updates or report problems.

When submitting feedback, please include:

* the pontoon number or location,
* the attribute you want to update,
* any relevant notes or observations,
* optional updated photos.

Possible contributions include:

* corrected location information
* new or updated photos
* missing locations
* updated information about shade, lawn condition, food options, or first aid
* general comments or improvements

## Future Plans

Possible future improvements include:

* adding more recreational locations
* updating field observations over time
* improving photo coverage
* adding more filter options
* improving mobile usability

## Created by

This dataset was enriched and the webmap created by:

* Pauline Fritz
* Lukas Preining
* Verena Damiani

Students of the University of Vienna.
As part of the Research Seminar Spatial Data Science and GeoCommunication.
