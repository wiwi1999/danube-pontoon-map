# Metadata: Cooling off on the Danube

## Description

This dataset contains selected recreational pontoon locations along the Donauinsel in Vienna. It was created for an interactive Leaflet web map and combines official open data, field-collected observations, and spatial analysis results.

## Data Sources

Original dataset: **Donauinsel Freizeiteinrichtungen Standorte Wien**  
Publisher: **City of Vienna / Stadt Wien**  
Source: https://www.data.gv.at/datasets/4e8d237b-8bd4-4483-a85d-431784c543b9?locale=de

Additional spatial analysis source: **GIP.at**  
Provider: **ÖVDAT**  
License: **Creative Commons Attribution 4.0 International (CC BY 4.0)**

## Data Collection and Processing

The original dataset was extended with field-collected information about shade, lawn or ground condition, chill area size, nudism area information, notes, and photos.

GIP.at was used to calculate approximate distances to nearby infrastructure such as first aid stations, restaurants, bistros, paths, and access routes. Distance values are stored in meters.

## Spatial Information

Geographic area: **Donauinsel, Vienna, Austria**  
Geometry type: **Point**  
Coordinate reference system: **WGS 84 / EPSG:4326**  
Data format: **GeoJSON**  
Main file: `data/pontoons.geojson`

## Attributes

| Field Name | Type | Description |
|---|---|---|
| `Index` | Integer | Unique identifier for each location; also used to link photos. |
| `CHILL_AREA` | Integer | Estimated chill area in square meters. |
| `SHADE` | Boolean coded as integer | `0` = no shade, `1` = shade available. |
| `LAWN` | Integer | Lawn or ground condition. `1` = mowed, `2` = medium height, `3` = high grass, `4` = sand/soil. |
| `LAWN_DATE` | Date | Date when the lawn or ground condition was recorded. |
| `NUDISM_ARE` | Text | Indicates whether the location is within or near a nudism area. |
| `DIST_FIRST` | Integer | Distance to the nearest first aid station in meters. |
| `DIST_FOOD` | Integer | Distance to the nearest restaurant or bistro in meters. |
| `NOTES` | Text | Additional observations or comments. |

## Photos

Photos are stored in the `pictures/` folder and linked by the `Index` field.

Example: `pictures/5.jpg` belongs to the feature with `Index` 5.

## License

This dataset is licensed under the **Creative Commons Attribution 4.0 International License (CC BY 4.0)**.

License text: https://creativecommons.org/licenses/by/4.0/deed.en

Changes were made to the original data. The dataset was enriched with field observations, additional attributes, photos, and spatial analysis results.

## Authors

Pauline Fritz, Lukas Preining, Verena Damiani  
Students of the University of Vienna
