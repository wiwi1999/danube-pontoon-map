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

| Attribute          | Description                                                     |
| ------------------ | --------------------------------------------------------------- |
| Pontoon ID         | Unique number of the location                                   |
| Chill Area         | Estimated available resting or chill area in square meters      |
| Shade              | Information about shade availability                            |
| Lawn               | Information about lawn availability                             |
| First Aid Distance | Approximate distance to the nearest first aid station           |
| Food Distance      | Approximate distance to the nearest restaurant, café, or bistro |
| Notes              | Additional observations about the location                      |
| Photo              | Image of the pontoon or surrounding area                        |

## Technologies Used

This project was built with:

* HTML
* CSS
* JavaScript
* Leaflet.js
* GeoJSON
* OpenStreetMap
* CARTO basemap
* ESRI satellite basemap

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
