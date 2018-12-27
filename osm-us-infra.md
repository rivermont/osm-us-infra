# United States Infrastructure Mapping
A good guide and standards do not currently exist for mapping the general utility infrastructure of the U.S.  
This document will serve as a dumping ground for ideas and content, until sections are sorted well and some are given their own pages.  

***

While infrastructure norms differ between countries, the U.S. is generally consistent across the states, thanks to standardization of products, cooperation between companies and contractors, and municipal laws. The U.S. is largely unmapped on a small scale, however.

See [[WikiProject Power networks/United States]].

[OpenInfraMap](https://github.com/openinframap/)

## Power Infrastructure
It is certainly possibly to map the grid from the coal plant all the way to the street light or house.  
However it is currently quite confusing trying to map all of the features.  
Almost all of the grid besides major lines is unmapped, and many different components do not have a tagging scheme created yet.

`power=line`, `power=minor_line`, `power=substation`, `power=generator` and many others.

https://www.youtube.com/watch?v=C8wCAbuSzUE

### Untagged
Things that need a tag created for them.

#### Power Meters (`power=meter`)
Goes well with `power=terminal` for homes, but is found at every traffic light, lit-up sign or other government-operated power-consuming device. When metering multiple devices or located away from the device it's monitoring, some relation could be created to link the two.

### Power Towers


### Power Poles

The [FHWA 1993 Highway/Utility Guide](https://www.fhwa.dot.gov/utilities/010604.pdf) ([Wayback](https://web.archive.org/web/*/https://www.fhwa.dot.gov/utilities/010604.pdf)) has some good insights into planning, pole space allocation, &c.

#### Shapes
`design=*`

### Other
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
[WiGLE](https://wigle.net) is a useful tool for mapping out cell and WiFi networks.
At some point a cell coverage map could be created using OSM data.

#### Wi-Fi and others
Free roadside WiFi access by providers like Spectrum, AT&T is attached to the lines and widespread. WiGLE is also useful here for determining coverage of different providers.  



### Traffic Lights
Street cabinets, refs on them, lights, cables, poles.

A schema describing light timing might be useful at some point.
Some way to indicate vehicle sensors (in-ground magenetic or vision).

Possibly a traffic light relation connecting sensors, lights, timing and control boxes.


### Street Lights
Currently, the most common way to tag street lights is simply a node with `highway=street_lamp`. Unless it is known, the type of light and other metadata are not usually added. This can be useful for data consumers and renderers, and is something that should be more widely added.  
[osmstreetlight.bplaced.net](http://osmstreetlight.bplaced.net) is a good example of a street light renderer.
Need much more detailed way to ID different `lamp_type`s.
Current tagging scheme is vague - `lamp_type=electric`??
How to identify in the daytime and nighttime - characteristics of the mount are easier to identify in daylight but the type of bulb is fast to ID at night.
Types of mounts and shrouds.
Daylight sensors, always-on or timed?

[A History of Street Lighting in the United States](en.wikipedia.org/wiki/History_of_street_lighting_in_the_United_States) on Wikipedia has a good overview of different types of lights and mounts, as well as many pictures of common light models.


# US Street Signs
A searchable, online database should be created for looking up street signs and their tagging. It should contain pictures, short descriptions, sign text and colors, and similar signs to be searchable. It should be easily editable (GitHub repo likely) and contain all of the MUTCD signs with variants as well as state and municipal additions.
  - Possibly expanded to be used for all street signs, not just U.S.

A good in-depth guide should be created for the correct way to tag street signs.  
There should be strong OpenStreetCam and Mapillary sign detection integration with projects like iD, and work should be put towards reducing false positives/negatives through model training.

# Miscellaneous Infrastructure
These things don't fit into the other categories but still need their own tagging system.

  - [Variable Message Sign](https://en.wikipedia.org/wiki/Variable-message_sign)
