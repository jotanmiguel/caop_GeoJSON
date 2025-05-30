# Portuguese Municipal Boundaries (2024)

This dataset provides a **cleaned, unified and ready-to-use GeoJSON file** with the boundaries of all Portuguese municipalities, including mainland Portugal, Madeira, and Azores.

## 🔹 Source
Based on original data from the public repository by [nmota](https://github.com/nmota/geoPortugal), who provides municipal and parish GeoJSONs derived from the **Carta Administrativa Oficial de Portugal (CAOP)** by the **Direção-Geral do Território**.

Projection systems were harmonized from:
- Mainland: PT-TM06/ETRS89  
- Madeira: PTRA08/UTM zone 28N  
- Azores Central & Eastern: PTRA08/UTM zone 26N  
- Azores Western: PTRA08/UTM zone 25N  

## 🔹 Processing Steps
- All 5 regional GeoJSONs were reprojected to **EPSG:4326 (WGS84)**.
- Geometry validity was ensured using `.buffer(0)` corrections.
- Properties were standardized (e.g., `DICO`, `Concelho`, `Distrito`).
- Resulting file is suitable for **Plotly, Folium, Leaflet, Power BI**, etc.

## 🔹 Suggested Uses
- Choropleth maps and spatial visualizations 
- Urban and regional analysis

## 🔹 Format
- File: `Portugal_Municipalities.geojson`  
- CRS: `EPSG:4326`  
- Geometry type: `Polygon` / `MultiPolygon`  
- Features: 308 municipalities  

## 🔹 Preview
![preview](https://i.ibb.co/ksgK1ysZ/output.png)

## 📎 License
Original data is open-source. This compiled version is distributed under **CC BY 4.0**, with attribution to [nmota](https://github.com/nmota/geoPortugal) and DGT Portugal.
