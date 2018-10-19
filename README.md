# Folium SemiCircle

[Folium](https://github.com/python-visualization/folium) is a Python porting for [Leaflet](http://leafletjs.com/), this is for include [SemiCircle](https://github.com/jieter/Leaflet-semicircle) plugin in Folium.

## Installation

Copy semicircle.py file in plugins directory of Folium library

## How it work

Like SemiCircle plugin there are two methods for call plugin:

Using `startAngle` and `stopAngle`:
```
Import folium
from folium import plugins
L.semiCircle([51.5, -0.09], {
    radius: 500,
	startAngle: 45,
	stopAngle: 135
}).addTo(map);
```
or using `direction` and `arc`:
```
L.semiCircle([51.5, -0.09], {
    radius: 500,
	startAngle: 45,
	stopAngle: 135
}).addTo(map);
```

## Screenshot

![](https://farm8.staticflickr.com/7373/12376158164_e335b4e61d_b.jpg)

## Jupyter Netbook Demo


## Change log
* 18.10.2018 - First edition
