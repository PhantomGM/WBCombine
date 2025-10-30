---
title: "Map View Quickstart"
type: "guide"
tags: [mapview, guide]
created: 2025-10-23
updated: 2025-10-23
---

# Obsidian **Map View** Quickstart

**Goal:** Use the Map View plugin to visualize notes (Settlements, Factions HQs, Landmarks) on a world map using latitude/longitude in frontmatter.

## 1) Install
- Install **Map View** plugin (Community Plugins → search “Map View”).
- Enable the plugin. A **map pin** icon should appear in the left ribbon.

## 2) Add Geo Fields to Notes
Include these fields in a note's frontmatter (YAML at the top):

```yaml
---
title: "Eastgate - Overview"
type: "settlement"
tags: [settlement]
latitude: 38.10
longitude: -23.60
---
```

> Tip: Add `type: settlement` or `type: faction` so dashboards and filters can group your pins.

## 3) Open the Map Panel
- Click the **Map View** ribbon icon; it will index notes that have `latitude` and `longitude`.
- Use **Filters** to show/hide by tag or folder (e.g. `07_NPCs`, `04_Settlements`).

## 4) Use the Dashboard
Open `[[Dashboards/Map_View_Dashboard]]` to see Dataview-powered lists of every note with coordinates. Clicking an item opens the note; **Map View** will show its pin.

## 5) Fantasy Worlds
Map View uses Earth-style coordinates. If you want **fantasy pixel maps**, use the Leaflet templates provided in the Leaflet add-on. You can use **both**: Leaflet for story maps, Map View for global index.

---

### FAQ
**Q:** Do I need a map tile key?  
**A:** No for local/offline defaults; Map View ships with basic tiles. For custom tiles, configure in plugin settings.

**Q:** Can I plot factions as well?  
**A:** Yes—add `latitude/longitude` to the faction’s HQ note.
