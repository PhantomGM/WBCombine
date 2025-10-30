---
title: "The Wild Reach (Leaflet Map)"
type: "map"
tags: [map, leaflet, region]
created: 2025-10-23
updated: 2025-10-23
---

# The Wild Reach — Interactive Map

Linked region: [[03_Regions/The_Wild_Reach/Region_Profile]]  
Replace `[[03_Regions/The_Wild_Reach/Assets/wild_reach_placeholder.png]]` with your region map.

```leaflet
id: wild-reach-map
image: [[03_Regions/The_Wild_Reach/Assets/wild_reach_placeholder.png]]
minZoom: -2
maxZoom: 5
defaultZoom: 0
bounds:
  - [0, 0]
  - [1600, 2400]
zoomDelta: 0.5
scale: true
marker:
  - coordinates: [900, 380] 
    icon: castle
    popup: "[[04_Settlements/Eastgate/Overview|Eastgate]]"
  - coordinates: [680, 1200]
    icon: waypoint
    popup: "[[08_Quests/The_Fogline_Pass/Summary|Quest: The Fogline Pass]]"
shape:
  - polyline:
      - [900, 380]
      - [760, 700]
      - [710, 960]
      - [680, 1200]
    color: orange
    weight: 3
    popup: "Expedition route to the fogline"
```
