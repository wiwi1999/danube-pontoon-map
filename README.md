# Cooling Off on the Danube

An interactive web map and enriched dataset of pontoons and recreational spots on Vienna’s Donauinsel.

## Project Overview

**Cooling Off on the Danube** is a web map and dataset about pontoons on Vienna’s Donauinsel. The aim of the project is to make it easier to choose suitable chill and resting spots on the island, one of Vienna’s most important recreational areas during hot summer days.

The project provides both:

* an interactive Leaflet web map for exploring pontoon locations, and
* an enriched dataset that can be reused for spatial analysis, visualization, or further research.

The original open data was extended with project-specific information such as shade availability, lawn or ground condition, estimated chill area, nudism area information, distances to nearby infrastructure, and photos.

## Dataset Information

Dataset created: `ADD_DATE_HERE`
Field observations collected: `06.,09.,13. June 2026`
Last updated: `19.06.2026`

## Web Map

Check out the interactive map here:

**[Cooling Off on the Danube](ADD_MAP_LINK_HERE)**

The map includes:

* interactive markers for pontoon locations,
* popups with detailed information and photos,
* filters for shade, lawn availability, nudism area information, and minimum chill area,
* multiple basemaps, including OpenStreetMap, Carto Light, and ESRI Satellite,
* a feedback button for suggesting updates or corrections.

## Feedback and Contributions

The map includes a GitHub issue button that allows users to suggest updates or report problems.

When submitting feedback, please include:

* the pontoon number or location,
* the attribute you want to update,
* any relevant notes or observations,
* optional updated photos.

Possible contributions include:

* corrected location information,
* new or updated photos,
* missing locations,
* changed access conditions,
* updated information about shade, lawn condition, food options, or first aid,
* general comments or improvements.

## Data Sources

The original data used in this project comes from the dataset **“Donauinsel Freizeiteinrichtungen Standorte Wien”**, published by the **City of Vienna / Stadt Wien** on the Austrian Open Government Data portal **data.gv.at**.

Original dataset:

**Donauinsel Freizeiteinrichtungen Standorte Wien**
Published by: **City of Vienna / Stadt Wien**
License: **Creative Commons Attribution 4.0 International — CC BY 4.0**

For this project, the original dataset was enriched with field-collected observations and additional analysis results.

For the network analysis, **GIP.at** was used to calculate approximate network-based distances to nearby infrastructure such as first aid stations, restaurants, bistros, paths, and access routes.

GIP data is provided by **ÖVDAT** and is available under the **Creative Commons Attribution 4.0 International — CC BY 4.0** license.

## Data Collection and Network Analysis

The final dataset combines:

* official open data from the City of Vienna,
* field-collected observations,
* manually added photos,
* network analysis based on GIP.at / ÖVDAT data.

Field observations include information about:

* shade availability,
* lawn or ground condition,
* estimated chill or resting area,
* nudism area information,
* photos.

Network analysis was used to calculate approximate distances to nearby infrastructure such as first aid stations and restaurants or bistros. These distances should be used for orientation only.

## Dataset Attributes

| Attribute     | Type                     | Description                                                                                 |
| ------------- | ------------------------ | ------------------------------------------------------------------------------------------- |
| `ORTBESCHR`   | Text                     | Original location description from the source dataset.                                      |
| `CHILL_AREA`  | Number                   | Estimated available chill or resting area in square meters.                                 |
| `SHADE`       | Boolean coded as integer | Shade availability. `0` = no shade, `1` = shade available.                                  |
| `LAWN`        | Categorical integer      | Lawn or ground condition recorded during field collection.                                  |
| `c_lat`       | Number                   | Latitude coordinate used for map display.                                                   |
| `c_lon`       | Number                   | Longitude coordinate used for map display.                                                  |
| `lawn_date`   | Date                     | Date when the lawn or ground condition was recorded.                                        |
| `lawn_text`   | Text                     | Text version of the lawn or ground condition category.                                      |
| `nudism_area` | Text                     | Indicates whether the location is within or near a nudism area.                             |
| `dist_first`  | Number                   | Approximate network-based distance to the nearest first aid station, measured in meters.    |
| `dist_food`   | Number                   | Approximate network-based distance to the nearest restaurant or bistro, measured in meters. |

## Usage

The dataset can be used to:

* explore recreational infrastructure on the Donauinsel,
* compare pontoon locations based on shade, lawn condition, and available chill area,
* identify nearby food or first aid infrastructure,
* support further spatial or network-based analysis,
* update or improve the interactive web map.

## Limitations

Some information is based on observation or estimation and may change over time.

Distances are approximate and should be used for orientation only. Shade availability can vary depending on the time of day, season, weather, and surrounding vegetation.

## Credits

Created by:

* Pauline Fritz
* Lukas Preining
* Verena Damiani

Students of the University of Vienna.

This project uses open data from the **City of Vienna / Stadt Wien** and **GIP.at / ÖVDAT** data for network analysis.

## License and Attribution

This project is based on open data from the **City of Vienna / Stadt Wien**, dataset **“Donauinsel Freizeiteinrichtungen Standorte Wien”**, licensed under **Creative Commons Attribution 4.0 International — CC BY 4.0**.

Users of this dataset must credit the **City of Vienna / Stadt Wien** as the original data source.

GIP.at data used for network analysis is provided by **ÖVDAT** and licensed under **Creative Commons Attribution 4.0 International — CC BY 4.0**.

Additional project-specific observations, photos, and derived attributes were collected and added by the project team.

## Future Plans

Possible future improvements include:

* adding more pontoons and recreational locations,
* updating field observations over time,
* improving photo coverage,
* adding more filter options,
* improving mobile usability,

