# Green Corner 🌱

A one-file web app for **NASA Space Apps Challenge 2026** (The Earth Information Jukebox).
Green Corner turns NASA Earth data into sound (**sonification**), so you can *listen* to how green, warm and rainy a place is before you see the numbers.

Ứng dụng web một file cho **NASA Space Apps Challenge 2026**: biến dữ liệu Trái Đất của NASA thành âm thanh.

**Play / Chơi:** https://mlink1415.github.io/green-corner-app/

## How it works

- 🌳 Plant greenness (NDVI) → piano
- 🌡️ Temperature → crickets (Dolbear's law)
- 🌧️ Rain → rain sound (+ thunder when it rains a lot)

All sounds are synthesized in the browser with the Web Audio API. No recorded audio files are used.
Explore by place, by time (2006–2026), by month, or play 6 mini-games. Vietnamese / English.

## Data sources and credits

| Source | Used for | License / terms |
|---|---|---|
| [NASA POWER](https://power.larc.nasa.gov/) (monthly point API) | Temperature, rainfall, soil moisture | NASA open data |
| [MODIS MOD13Q1 NDVI](https://lpdaac.usgs.gov/products/mod13q1v061/) via [ORNL DAAC MODIS Web Service](https://modis.ornl.gov/data/modis_webservice.html) | Plant greenness | NASA open data |
| [NASA Worldview Snapshots / GIBS](https://worldview.earthdata.nasa.gov/) (VIIRS, MODIS) | Satellite photos | NASA open data |
| [NASA Blue Marble Next Generation](https://visibleearth.nasa.gov/collection/1484/blue-marble) | Globe texture, mystery photos | NASA open data |
| [Natural Earth](https://www.naturalearthdata.com/) 110m via [world-atlas](https://github.com/topojson/world-atlas) | World map shapes (embedded) | Public domain / ISC |
| [i18n-iso-countries](https://github.com/michaelwittig/node-i18n-iso-countries) | Country codes (embedded) | MIT |
| [Open-Meteo Geocoding API](https://open-meteo.com/en/docs/geocoding-api) (data from [GeoNames](https://www.geonames.org/)) | City search | CC BY 4.0 |

Time-mode monthly series for 8 places were prepared from NASA POWER and MODIS data.
