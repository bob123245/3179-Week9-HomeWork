{
    "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
    "title": "Australia people destribution ",
    "width": 800,
    "height": 600,
    "projection": {"type": "equirectangular"},
    "data": {
    "url": "https://raw.githubusercontent.com/bob123245/3179-Week9-HomeWork/master/STE_2021_AUST_GDA2020.json",
    "format": {"type": "topojson", "feature": "STE_2021_AUST_GDA2020"}
    },
    "transform": [
    {
    "lookup": "properties.STE_NAME21",
    "from": {
    "data": {
    "url": "https://raw.githubusercontent.com/bob123245/3179-Week9-HomeWork/master/au.csv"
    },  
   "key": "admin_name",
    "fields": ["population"]
    }
    }
    ],
    "mark": {"type": "geoshape"},
    "encoding": {
    "color": {
    "field": "population",
    "type": "quantitative",
    "scale": {
    "type": "threshold",
    "domain": [500, 1000, 2000],
    "range": ["#fdbe85", "#fd8d3c", "#e6550d", "#a63603"]
    }
   
    },
    "tooltip": [
    {"field": "properties.STE_NAME21", "type": "nominal", "title": "Country"},
    {"field": "population", "type": "quantitative"}
    ]
    }
   }
