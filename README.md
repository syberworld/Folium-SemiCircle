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

![](https://farm8.staticflickr.com/7373/12376158164_e335b4e61d_b.jpg)

## Jupyter Netbook Demo


## Change log
* 18.10.2018 - First edition
