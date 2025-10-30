---
title: "Map View - Custom Offline World Map"
type: "mapview"
tags: [mapview, custom, world]
created: 2025-10-23
updated: 2025-10-23
---

# 🗺️ Map View — Custom Offline World Map

This setup uses your own image (`[[02_World/Assets/world_map_placeholder.png]]`) as the base for Map View.  
This method works **offline** and uses **fictional coordinates** instead of Earth lat/long.

---

## ⚙️ Setup Instructions

1. Open **Settings → Map View → Map Provider** → select **Custom Map Image**.  
2. When prompted, choose your image file:  
   `02_World/Assets/world_map_placeholder.png`
3. In **Settings → Map View → Bounds**, set example values:  
   - North: `100`  
   - South: `-100`  
   - West: `-200`  
   - East: `200`  
   (This gives you a coordinate grid of -200 → 200 longitude and -100 → 100 latitude.)
4. Set your **Default View** (center) to:  
   - Latitude: `0`  
   - Longitude: `0`  
   - Zoom: `0.5`  

> You can scale or move your pins anywhere on this grid — treat it like your own world coordinate system.

---

## 📍 Sample Notes with Coordinates

Below are examples of notes with coordinates for this offline fantasy map system.

```yaml
---
title: "Eastgate - Overview"
type: "settlement"
tags: [settlement, eastgate]
latitude: 20
longitude: -40
---
```

```yaml
---
title: "Wanderers Guild - Overview"
type: "faction"
tags: [faction, guild]
latitude: 25
longitude: -30
---
```

```yaml
---
title: "The Wild Reach - Region Profile"
type: "region"
tags: [region]
latitude: 15
longitude: -60
---
```

---

## 🧭 Linking Map View and Leaflet
- `[[02_World/World_Map_Leaflet]]` → opens zoomable version via Leaflet plugin.  
- This Map View layout provides the **overview grid**, while Leaflet handles **detailed exploration.**

---

### ✅ Summary
- Fully offline.  
- Uses your fantasy world map image.  
- Custom coordinate grid.  
- Compatible with Dataview tables and Map View pins.

> Once configured, any note with `latitude` and `longitude` will appear as a pin on your image map.
