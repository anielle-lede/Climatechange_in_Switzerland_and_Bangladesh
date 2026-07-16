# What One Degree Looks Like — Switzerland and Bangladesh

A scrollytelling data story comparing how the same amount of global warming plays out in two very different countries: melting glaciers and thawing permafrost in Switzerland, and rising seas and worsening floods in Bangladesh.

**Live site:** https://anielle-lede.github.io/Climatechange_in_Switzerland_and_Bangladesh/

## What's in this project

- **Switzerland:** glacier volume loss (Swiss Glacier Inventory, GLAMOS/SGI), permafrost ground temperatures (PERMOS monitoring network), and the 2025 Blatten rockslide.
- **Bangladesh:** flood risk mapping (BARC/SPARRSO via the Humanitarian Data Exchange), sea level anomaly in the Bay of Bengal (NOAA Laboratory for Satellite Altimetry), and annual precipitation in Dhaka (NASA POWER).

Full methodology and sources are documented in a box at the bottom of the page itself.

## Built with

- [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/) for the maps
- [D3.js](https://d3js.org/) for the time series charts
- [Scrollama](https://github.com/russellgoldenberg/scrollama) for scroll-driven map steps
- Data processing in Python (pandas, geopandas)

## Methodology 

Glacier volume loss from the Swiss Glacier Inventory (GLAMOS/SGI). Permafrost ground temperatures from the PERMOS monitoring network, filtered to ~10m depth (the standard reference depth in permafrost research), averaged per site and year.

Flood risk from a hazard map by the Bangladesh Agricultural Research Council (BARC/SPARRSO, via the Humanitarian Data Exchange). Sea level anomaly from satellite data by the NOAA Laboratory for Satellite Altimetry (Bay of Bengal, since 1993). Precipitation from NASA POWER satellite data for Dhaka.

All raw data was cleaned in Python (pandas/geopandas): tables were merged, filtered to reference depths or complete years, aggregated into annual values, and, for precipitation, converted from daily to annual totals. Missing measurement years are shown in the charts as dashed lines, not hidden.

Maps built with Mapbox GL JS (including national borders, scroll behavior, and zoom controls), time series charts built with D3.js (scroll-triggered animation, interactive tooltips, data gaps shown as dashed lines).

## Inspiration

https://www.nytimes.com/interactive/2020/12/17/world/asia/india-pollution-inequality.html
