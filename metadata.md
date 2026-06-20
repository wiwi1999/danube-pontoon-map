# Metadata: Cooling Off on the Danube

## Description

This dataset contains selected recreational pontoon locations along the Donauinsel in Vienna, Austria. It was created for an interactive Leaflet web map and combines official open data, field-collected observations, photos, and network analysis results.

## Dataset Information

Dataset created: `June 2026`
Field observations collected: `6, 9, and 13 June 2026`
Last updated: `19 June 2026`

## Data Sources

Original dataset:

Stadt Wien. (2025). Donauinsel Freizeiteinrichtungen Standorte Wien [Data set]. data.gv.at.
https://www.data.gv.at/datasets/4e8d237b-8bd4-4483-a85d-431784c543b9?locale=de

Network analysis data:

ÖVDAT. (2026). GIP / Graphenintegrations-Plattform Österreich [Data set]. data.gv.at.
https://www.data.gv.at/katalog/dataset/3fefc838-791d-4dde-975b-a4131a54e7c5


## License and Attribution

The original datasets are licensed under Creative Commons Attribution 4.0 International — CC BY 4.0.

License text:
https://creativecommons.org/licenses/by/4.0/

Attribution for the City of Vienna dataset:

> Stadt Wien – data.wien.gv.at

Attribution for the GIP dataset:

> ÖVDAT/GIP.at – Graphenintegrations-Plattform Österreich

This derived dataset includes changes to the original data. It was enriched with field-collected observations, additional attributes, photos, and spatial analysis results.

Users of this dataset must credit this derived dataset as well as the original data sources listed above.

## Data Collection and Processing

The original dataset was extended with field-collected information about shade availability, lawn or ground condition, estimated chill area size, nudism area information, and photos.

GIP.at data was used for network analysis to calculate approximate network-based distances to nearby infrastructure such as first aid stations, restaurants, bistros, paths, and access routes. Distance values are stored in meters.

## Spatial Information

Geographic area: **Donauinsel, Vienna, Austria**
Geometry type: **Point**
Coordinate reference system: **WGS 84 / EPSG:4326**
Data format: **GeoJSON**
Main file: `data/pontoons.geojson`

## Attributes

| Field Name    | Type                     | Description                                                                                                                     |
| ------------- | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------- |
| `ORTBESCHR`   | Text                     | Original location description from the source dataset.                                                                          |
| `CHILL_AREA`  | Number                   | Estimated available chill or resting area in square meters.                                                                     |
| `SHADE`       | Boolean coded as integer | Shade availability. `0` = no shade, `1` = shade available.                                                                      |
| `LAWN`        | Categorical integer      | Lawn or ground condition recorded during field collection. `1` = mowed, `2` = medium height, `3` = high grass, `4` = sand/soil. |
| `c_lat`       | Number                   | Latitude coordinate used for map display.                                                                                       |
| `c_lon`       | Number                   | Longitude coordinate used for map display.                                                                                      |
| `lawn_date`   | Date                     | Date when the lawn or ground condition was recorded.                                                                            |
| `lawn_text`   | Text                     | Text version of the lawn or ground condition category, for example “mowed”, “medium height”, “high grass”, or “sand/soil”.      |
| `nudism_area` | Text                     | Indicates whether the location is within or near a nudism area.                                                                 |
| `dist_first`  | Number                   | Approximate network-based distance to the nearest first aid station, measured in meters.                                        |
| `dist_food`   | Number                   | Approximate network-based distance to the nearest restaurant or bistro, measured in meters.                                     |

## Photos

Photos are stored in the `pictures/` folder and linked to the corresponding locations through the dataset.

Example: a photo named `pictures/5.jpg` belongs to the corresponding feature or pontoon location with the matching identifier used in the project.

## Limitations

Some information is based on observation or estimation and may change over time. Network-based distances are approximate and should be used for orientation only. Shade availability can vary depending on the time of day, season, weather, and surrounding vegetation.

## Authors

* Pauline Fritz
* Lukas Preining
* Verena Damiani

Students of the University of Vienna.
As part of the Research Seminar Spatial Data Science and GeoCommunication.
