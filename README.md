# Folium SemiCircle

[Folium](https://github.com/python-visualization/folium) is a Python porting for [Leaflet](http://leafletjs.com/), this is for include [SemiCircle](https://github.com/jieter/Leaflet-semicircle) plugin in Folium.

## Installation

Copy semicircle.py file in plugins directory of Folium library

Add to __init__.py in plugins directory refer to plugin

## How it work

Like SemiCircle plugin there are two methods for call plugin:

Using `startAngle` and `stopAngle`:
```
import folium
from folium import plugins
m = folium.Map(
    location=[39.217, 9.136],
    zoom_start=14,
    tiles='Stamen Terrain'
)
plugins.SemiCircle(
    location=[39.217, 9.136],   # Location of center
    radius= 1500,               # Radius in meters
    startAngle= 10,             # Start angle (0 to 360 degrees)
    stopAngle=100               # Stop angle (0 to 360 degrees)
).add_to(m)
```
or using `direction` and `arc`:
```
import folium
from folium import plugins
m = folium.Map(
    location=[39.217, 9.136],
    zoom_start=14,
    tiles='Stamen Terrain'
)
plugins.SemiCircle(
    location=[39.217, 9.136],   # Location of center
    radius= 1500,               # Radius in meters
    direction= 270,             # Direction of cone center (0 to 360 degrees)
    arc=90                      # Amplitude of cone (0 to 360 degrees)
).add_to(m)
```

## Screenshot

![](https://raw.githubusercontent.com/syberworld/Folium-SemiCircle/master/Screenshot.png)

## Jupyter Netbook Demo

You can see a demo at [this link](http://nbviewer.jupyter.org/github/syberworld/Folium-SemiCircle/blob/master/Folium%20SemiCircle.ipynb)

## Change log
* 18.10.2018 - First edition
