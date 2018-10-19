# Folium SemiCircle

[Folium](https://github.com/python-visualization/folium) is a Python porting for [Leaflet](http://leafletjs.com/), this is for include [SemiCircle](https://github.com/jieter/Leaflet-semicircle) plugin in Folium.

## Installation

Copy semicircle.py file in plugins directory of Folium library

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
    location=[39.217, 9.136],
    radius= 1500,
    startAngle= 10,
    stopAngle=100
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
    location=[39.217, 9.136],
    radius= 1500,
    direction= 270,
    arc=90
).add_to(m)
```

## Screenshot

![](https://raw.githubusercontent.com/syberworld/Folium-SemiCircle/master/Screenshot.png)

## Jupyter Netbook Demo

You can see a demo at [this link](http://nbviewer.jupyter.org/github/syberworld/Folium-SemiCircle/blob/master/Folium%20SemiCircle.ipynb)

## Change log
* 18.10.2018 - First edition
