
> [!NOTE]- Quick Calculator  
> Map Height in Pixels: `INPUT[number:map_height_y]`  
> Map Width in Pixels: `INPUT[number:map_width_x]`  
> lat: `VIEW[{map_height_y} / 2][math]`  
> long: `VIEW[{map_width_x} / 2][math]`  
> How Many Pixels In Scale: `INPUT[number:scale_pixels]`  
> How Many Units in Scale: `INPUT[number:scale_pixels_range]`  
> Scale: `VIEW[1/({scale_pixels}/{scale_pixels_range})][math:mapCalc1]`



```leaflet  
id: world-map
image: [[02_World/Assets/world_map_placeholder.png]]
bounds:
  - [1024, 0]      # bottom-left (y, x)
  - [0, 1536]      # top-right   (y, x)
center: [512, 768]  # [height/2, width/2]
minZoom: -2
maxZoom: 5
defaultZoom: -1
noWrap: true

```
