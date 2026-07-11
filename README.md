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

## Running locally

```
python3 -m http.server
```

Then open `http://localhost:8000` in a browser.
