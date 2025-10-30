---
title: "World Map (Leaflet)"
type: "map"
tags: [map, leaflet, world]
created: 2025-10-23
updated: 2025-10-23
---

# World Map (Leaflet)

Install the **Obsidian Leaflet** plugin, then this map renders below.  
Replace the image `[[02_World/Assets/world_map_placeholder.png]]` with your real map (same filename).  
Use pixel coordinates for markers within the `bounds` size.

```leaflet
id: world-map
image: [[02_World/Assets/world_map_placeholder.png]]
bounds:
  - [0, 0]         # top-left (y, x)
  - [1024, 1536]   # bottom-right = [height, width]
center: [512, 768]  # center = [height/2, width/2]
minZoom: -2
maxZoom: 5
defaultZoom: -2     # try -2 if you want the whole map in view on load
noWrap: true

```
