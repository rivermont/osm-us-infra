While infrastructure norms differ between countries, the U.S. is generally consistent across the states, thanks to standardization of products, cooperation between companies and contractors, and municipal laws. The U.S. is largely unmapped on a small scale, however.

See [[WikiProject Power networks/United States]].

[OpenInfraMap](https://github.com/openinframap/)

## Power Infrastructure

`power=line`, `power=minor_line`, `power=substation`, `power=generator` and many others.

https://www.youtube.com/watch?v=C8wCAbuSzUE

### Power Towers


### Power Poles

#### Shapes
`design=*`

#### Stuff Attached to them
Transformers, street cabinets, cell, wifi, compensators, insulators.


## Pipeline Infrastructure
Sewer, water (storm sewer, potable and non-potable freshwater, aqueducts), natural gas etc.

## Utility Infrastructure
Telephone lines, internet and other services.

Street cabinets; how to differentiate between cable, fiber, phone.

### Wireless

#### Cell
Cell towers - possibly integration with OpenCellID somehow?
**Small cell tagging needs created**, they are widespread in some areas.
WiGLE is a useful tool for mapping out cell and WiFi networks.
At some point a cell coverage map could be created using OSM data.

#### Wi-Fi and others
Free roadside WiFi access by providers like Spectrum, AT&T is attached to the lines and widespread.


### Traffic Lights
Street cabinets, refs on them, lights, cables, poles.

A schema describing light timing might be useful at some point.
Some way to indicate vehicle sensors (in-ground magenetic or vision).

Possibly a traffic light relation connecting sensors, lights, timing and control boxes.


### Street Lights
Need much more detailed way to ID different `lamp_type`s.
Current tagging scheme is vague - `lamp_type=electric`??
How to identify in the daytime and nighttime.
Types of mounts and shrouds.
Daylight sensors, always-on or timed?


# US Street Signs
How to tag, what signs to tag.
MUTCD, state and local supplements.
OpenStreetCam (and Mapillary?) and what signs they detect.
