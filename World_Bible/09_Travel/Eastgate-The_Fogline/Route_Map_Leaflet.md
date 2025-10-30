---
title: "Travel: Eastgate → The Fogline (Leaflet)"
type: "map"
tags: [map, leaflet, travel]
created: 2025-10-23
updated: 2025-10-23
---

# Travel: Eastgate → The Fogline

Related notes: [[09_Travel/Eastgate-The_Fogline/Environment_Profile]] | [[09_Travel/Eastgate-The_Fogline/Hazards_and_Encounters]]

```leaflet
id: route-fogline
image: [[09_Travel/Eastgate-The_Fogline/Assets/route_map_placeholder.png]]
minZoom: -1
maxZoom: 5
defaultZoom: 0
bounds:
  - [0, 0]
  - [1400, 2000]
zoomDelta: 0.5
marker:
  - coordinates: [420, 300]
    icon: castle
    popup: "[[04_Settlements/Eastgate/Overview|Eastgate]]"
  - coordinates: [1050, 1500]
    icon: mountain
    popup: "Fogline ridge"
shape:
  - polyline:
      - [420, 300]
      - [650, 540]
      - [820, 820]
      - [960, 1160]
      - [1050, 1500]
    weight: 4
    color: blue
    popup: "Scouted path"
  - rectangle:
      - [820, 820]
      - [980, 1000]
    color: yellow
    weight: 2
    popup: "Hazard zone"
```
