# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]
- Use WFS on the perimeter map instead of WMS for the choosen products if available.
- Better default names for saved orders (perimeter-type? location?, product?, formats?)

## [1.0.3] - 2020-03-04
### Added
- It is now possible to start the application with the url parameter '?order={...}'. The given order is shown in the 'Bestellungen' list as '+++ Bestellung über URL-Parameter +++' and can be reloaded and changed. The JSON order has this structure:
- {
    "order_id": "f627b14917174c08a6ca3e8124faaf90",
    "internal_id": 260463,
    "status": "SUCCESS:Data transfer succeeded",
    "status_code": 200,
    "submitted": "2019-06-09T12:25:03",
    "finished": "2019-06-09T12:25:41",
    "order": {
        "email": "",
        "pdir_coordsys": "LV95",
        "pdir_polygon": {
            "coordinates": [
                [
                    [
                        2698167.0407617167,
                        1256591.8630807488
                    ],
                    [
                        2698719.9180706767,
                        1256591.8630807488
                    ],
                    [
                        2698719.9180706767,
                        1257294.095871276
                    ],
                    [
                        2698167.0407617167,
                        1257294.095871276
                    ],
                    [
                        2698167.0407617167,
                        1256591.8630807488
                    ]
                ]
            ],
            "type": "Polygon"
        },
        "perimeter_type": "DIRECT",
        "pindir_ident": [
            ""
        ],
        "pindir_layer_name": "COMMUNE",
        "products": [
            {
                "format_id": 1,
                "product_id": 277
            }
        ]
    },
    "orderTitle": "",
    "lots": []
}
- A possible link looks like this: [https://szinggeler.github.io/geoTangle/geotangle.html?order={%20"order_id":%20"f627b14917174c08a6ca3e8124faaf90",%20"internal_id":%20260463,%20"status":%20"SUCCESS:Data%20transfer%20succeeded",%20"status_code":%20200,%20"submitted":%20"2019-06-09T12:25:03",%20"finished":%20"2019-06-09T12:25:41",%20"order":%20{%20"email":%20"",%20"pdir_coordsys":%20"LV95",%20"pdir_polygon":%20{%20"coordinates":%20[%20[%20[%202698167.0407617167,%201256591.8630807488%20],%20[%202698719.9180706767,%201256591.8630807488%20],%20[%202698719.9180706767,%201257294.095871276%20],%20[%202698167.0407617167,%201257294.095871276%20],%20[%202698167.0407617167,%201256591.8630807488%20]%20]%20],%20"type":%20"Polygon"%20},%20"perimeter_type":%20"DIRECT",%20"pindir_ident":%20[%20""%20],%20"pindir_layer_name":%20"COMMUNE",%20"products":%20[{%20"format_id":%201,%20"product_id":%20277%20}]%20},%20"orderTitle":%20"",%20"lots":%20[]%20}](https://szinggeler.github.io/geoTangle/geotangle.html?order={%20"order_id":%20"f627b14917174c08a6ca3e8124faaf90",%20"internal_id":%20260463,%20"status":%20"SUCCESS:Data%20transfer%20succeeded",%20"status_code":%20200,%20"submitted":%20"2019-06-09T12:25:03",%20"finished":%20"2019-06-09T12:25:41",%20"order":%20{%20"email":%20"",%20"pdir_coordsys":%20"LV95",%20"pdir_polygon":%20{%20"coordinates":%20[%20[%20[%202698167.0407617167,%201256591.8630807488%20],%20[%202698719.9180706767,%201256591.8630807488%20],%20[%202698719.9180706767,%201257294.095871276%20],%20[%202698167.0407617167,%201257294.095871276%20],%20[%202698167.0407617167,%201256591.8630807488%20]%20]%20],%20"type":%20"Polygon"%20},%20"perimeter_type":%20"DIRECT",%20"pindir_ident":%20[%20""%20],%20"pindir_layer_name":%20"COMMUNE",%20"products":%20[{%20"format_id":%201,%20"product_id":%20277%20}]%20},%20"orderTitle":%20"",%20"lots":%20[]%20})

## [1.0.2] - 2020-02-01
### Added
- Show an alert if the area of polygons and rectangles is smaller then 1 m2 and delete this perimeter.

## [1.0.1] - 2020-01-19
### Added
- Version number and link to CHANGELOG.md
- Show self intersections of polygon, invalidate perimeter with self intersecting polygon.

## [1.0.0] - 2020-01-06
### Added
- First version of application published [Open Geodata Shop ZH](https://szinggeler.github.io/geoTangle/geotangle.html).


[Unreleased]: Added-Changed-Deprecated-Removed-Fixed-Security

