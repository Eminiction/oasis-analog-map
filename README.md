# OASIS – Outpost for Antarctic Simulation of Interplanetary Settlements

**AGH Space Tech Team · NASA Space Apps Challenge 2026**

🌍 **Live map:** https://eminiction.github.io/oasis-analog-map/

OASIS identifies and characterizes the **Bunger Hills Oasis** in East Antarctica (~66°S, 100°E) as a terrestrial analog for future bases on the **Moon** and **Mars**. Bunger Hills is one of the largest ice-free areas in Antarctica (~950 km²) with bare rocky hills, ice-covered and saline lakes, extreme cold and very limited access, yet it is far less studied than better-known analogs such as the McMurdo Dry Valleys.

The interactive web map puts Bunger Hills next to two planetary sites:

| World | Site | Why it was chosen |
|---|---|---|
| 🌍 Earth | Bunger Hills Oasis, Antarctica | Large ice-free polar oasis, isolated, lakes studied as Mars-lake analogs |
| 🌑 Moon | Lunar south pole (Shackleton, Cabeus craters) | Water-ice cold traps, low Sun angle, a prime region for future bases |
| 🔴 Mars | Jezero Crater | Ancient lake basin with a river delta |

## Features

1. **Three linked maps**: NASA satellite and orbital data for each site. The Moon is shown from directly above the south pole (polar stereographic view, re-projected in the browser), with a contrast control for the dark polar terrain.
2. **Analog score**: 8 factors (temperature, terrain, surface material, water & ice, sunlight cycle, isolation, atmosphere, gravity & radiation), each scored 0–5 for how well Bunger Hills reproduces Moon and Mars conditions, with sources. Factors that Antarctica cannot reproduce are included on purpose so the score stays honest.
3. **OASIS outpost concept**: a modular, autonomous base in Bunger Hills deployed in this order: (1) power source, (2) communications, (3) hub module with the crew shelter for service visits, (4) science incl. ELF/Schumann-resonance sensors, (5) future robotics and regolith 3D printing. It is operated remotely and serviced seasonally. Module positions on the map are illustrative.

## Data sources

**NASA**
- [NASA GIBS](https://www.earthdata.nasa.gov/engage/open-data-services-software/earthdata-developer-portal/gibs-api): MODIS Terra true colour and land-surface temperature, ASTER GDEM shaded relief (NASA/METI)
- [NASA Moon Trek](https://trek.nasa.gov/moon/): LRO WAC global mosaic, LRO LOLA colour-shaded elevation
- [NASA Mars Trek](https://trek.nasa.gov/mars/): Viking MDIM 2.1 colour mosaic, MGS MOLA colour-shaded elevation
- Andersen et al. (1995), *A preliminary comparison of two perennially ice-covered lakes in Antarctica: Analogs of past Martian lacustrine environments*: [NTRS 19950035178](https://ntrs.nasa.gov/citations/19950035178)
- Rice (1992), *Antarctic lakes (above and beneath the ice sheet): Analogues for Mars*: [NTRS 19930010628](https://ntrs.nasa.gov/citations/19930010628)

**Other**
- Doran et al. (1996), *Climatology and implications for perennial lake ice occurrence at Bunger Hills Oasis, East Antarctica*, Antarctic Science 8(3): 289–296
- Esri World Imagery basemap (high-resolution view of Bunger Hills)

## Built with

- HTML, CSS, JavaScript (single file: `index.html`)
- [Leaflet](https://leafletjs.com/) (BSD-2): Earth and Mars maps
- [OpenLayers](https://openlayers.org/) (BSD-2) + [proj4js](http://proj4js.org/) (MIT): Moon polar view
- Hosted on GitHub Pages
- Fonts: Fira Sans and Overpass (Google Fonts, SIL Open Font License)

## Run or edit locally

No installation is needed. Download `index.html` and open it in a browser (an internet connection is required for the map tiles).

The scores, site markers and outpost modules are plain data lists at the top of the script in `index.html` (`FACTORS`, `SITES`, `MODULES`) and can be edited directly.

## Use of AI

The code in `index.html` and parts of the descriptive text (including this README) were written with the assistance of an AI assistant (Claude, Anthropic) and reviewed and adjusted by the team. Site selection, the outpost concept and the analog assessment are the team's own work. No AI-generated images, audio or video are used.

## Team

AGH Space Tech Team: Izabela Świca, Piotr Libudzki, Mikołaj Głód, Michał Para

---

*Student hackathon project. Not affiliated with or endorsed by NASA.*
