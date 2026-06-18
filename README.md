# Cooling off on the Danube

This is an interactive web map showing selected recreational pontoons along the Donauinsel in Vienna.

The project helps users find comfortable places to cool off, relax, and spend time near the water during hot days. The map focuses on practical comfort factors such as shade, lawn availability, chill area size, distance to first aid stations, distance to restaurants or bistros, nudism area information, notes, and photos.

## Project Overview

Vienna’s Donauinsel is an important public recreation area, especially during the summer. This web map provides an overview of selected pontoon locations and nearby recreational facilities, making it easier to compare different places before visiting them.

Each location is shown as a marker on the map. Users can click on a marker to open a popup with detailed information and a photo of the location.

## Live Map

View the map here:

[Cooling off on the Danube](YOUR-LINK-HERE)

## Features

The map includes:

* Interactive markers for pontoon locations
* Popups with detailed information and photos
* Filters for the attributes: shade, lawn availability, nudism area information, and minimum chill area
* Multiple basemaps, including OpenStreetMap, Carto Light, and ESRI Satellite
* A feedback button that allows users to suggest updates or corrections

## Data Source

The original data used in this project comes from the dataset “Donauinsel Freizeiteinrichtungen Standorte Wien”, published by the City of Vienna on the Austrian Open Government Data portal **data.gv.at**.

Dataset source:

[Donauinsel Freizeiteinrichtungen Standorte Wien](https://www.data.gv.at/datasets/4e8d237b-8bd4-4483-a85d-431784c543b9?locale=de)

For this project, the original dataset was enriched with project-specific attributes, including information about shade, lawn availability, chill area size, distance to first aid stations, distance to restaurants or bistros, notes, and photos.

## Data Collection and Spatial Analysis

This project is based on official open data from the **City of Vienna / Stadt Wien**, published on **data.gv.at** as the dataset **“Donauinsel Freizeiteinrichtungen Standorte Wien”**.

The original data was extended with field-collected information, including observations about shade, lawn availability, chill area size, nudism area information, notes, and photos.

For spatial analysis, **GIP.at** was used as a reference dataset to calculate approximate distances to nearby infrastructure such as first aid stations, restaurants, bistros, paths, and access routes.

GIP data is provided by **ÖVDAT** and is available under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.

The final dataset combines official open data, field observations, and spatial analysis results for use in an interactive Leaflet web map.

## Attribute Description

The following table describes the attributes stored in the project GeoJSON dataset.

| Field Name      | Type                     | Description                                                                                                                             |
| --------------- | ------------------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| `Index`         | Integer                  | Unique identifier for each pontoon or location. Also used to link photos to map features.                                               |
| `CHILL_AREA`    | Number                   | Estimated available chill or resting area in square meters.                                                                             |
| `SHADE`         | Boolean coded as integer | Shade availability. `0` = no shade, `1` = shade available.                                                                              |
| `RASEN_ZUSTAND` | Categorical integer      | Lawn or ground condition recorded during field collection. `1` = mowed, `2` = medium height, `3` = high grass, `4` = sand/soil.         |
| `RASEN_DATUM`   | Date                     | Date when the lawn or ground condition was recorded. This field is used for documentation and does not necessarily appear in the popup. |
| `NUDISM_ARE`    | Text                     | Indicates whether the location is within or near a nudism area.                                                                         |
| `DIST_FIRST`    | Number                   | Distance to the nearest first aid station, measured in meters.                                                                          |
| `DIST_FOOD`     | Number                   | Distance to the nearest restaurant or bistro, measured in meters.                                                                       |
| `NOTES`         | Text                     | Additional observations or comments about the location.                                                                                 |

The popup presents selected attributes in a more readable form, while the attribute table documents the actual structure of the dataset.


## Map Filters

Users can filter the locations by the following criteria:

| Filter             | Description                                                     |
| ------------------ | --------------------------------------------------------------- |
| Shade              | Shows locations where shade is available                        |
| Lawn               | Shows locations with nearby lawn areas                          |
| Nudism Area        | Filters locations based on nudism area information              |
| Minimum Chill Area | Shows only locations with at least the selected chill area size |

## Popup Information

Each popup contains the following information:

## Popup Information

Each popup shows a simplified, user-friendly version of selected dataset attributes.

| Popup Label                   | Based on Dataset Field | Description                                                                                            |
| ----------------------------- | ---------------------- | ------------------------------------------------------------------------------------------------------ |
| Pontoon                       | `Index`                | Unique number of the pontoon or location.                                                              |
| Chill Area                    | `CHILL_AREA`           | Estimated available chill or resting area in square meters.                                            |
| Shade                         | `SHADE`                | Shows whether shade is available. The dataset stores this as `0` = no shade and `1` = shade available. |
| Lawn Condition                | `RASEN_ZUSTAND`        | Shows the field-recorded lawn or ground condition in a readable form.                                  |
| Distance to First Aid Station | `DIST_FIRST`           | Approximate distance to the nearest first aid station, in meters.                                      |
| Distance to Restaurant/Bistro | `DIST_FOOD`            | Approximate distance to the nearest restaurant or bistro, in meters.                                   |
| Nudism Area                   | `NUDISM_ARE`           | Indicates whether the location is within or near a nudism area.                                        |
| Notes                         | `NOTES`                | Additional observations about the location.                                                            |
| Photo                         | `Index`                | Photos are linked to each location using the `Index` value.                                            


## File Structure

```text
danube-pontoon-map/
│
├── index.html
├── css/
│   └── style.css
├── data/
│   └── pontoons.geojson
├── pictures/
│   ├── 1.jpg
│   ├── 2.jpg
│   └── ...
├── README.md
└── metadata.md
```

## How to Use the Project Locally

1. Download or clone this repository.
2. Open the project folder in a code editor.
3. Start a local server, for example with the Live Server extension in Visual Studio Code.
4. Open `index.html` in a browser.
5. Explore the map and use the filters.

A local server is recommended because some browsers block GeoJSON files when opening the HTML file directly.

## Contributions

Users can suggest updates or corrections through the feedback button on the map.

Possible contributions include:

* corrected location information
* new or updated photos
* missing locations
* changed access conditions
* updated information about shade, lawn, food options, or first aid
* general comments or improvements

## Limitations

The dataset may not include every pontoon or recreational facility along the Danube Island. Some information is based on observation or estimation and may change over time.

Distances are approximate and should be used for orientation only. Shade availability can vary depending on the time of day, season, and surrounding vegetation. Users should always follow local signs, safety rules, and official regulations on site.

## Attribution

This project uses open data provided by the City of Vienna and published through data.gv.at.

Original dataset: **Donauinsel Freizeiteinrichtungen Standorte Wien**
Publisher: **City of Vienna / Stadt Wien**
Source: [data.gv.at](https://www.data.gv.at/datasets/4e8d237b-8bd4-4483-a85d-431784c543b9?locale=de)

This project is an independent student web mapping project and is not an official product of the City of Vienna.

## Author

Pauline Fritz, Lukas Preining, Verena Damiani. Students of the University of Vienna.

## License

XX
