# EcoTrace: Bangalore Waste Mapping Platform

EcoTrace is a civic-tech website that makes Bangalore's waste problem easier to see and act on. It shows waste hotspots on an interactive map, lets residents search dry waste collection centres by zone, and explains how to segregate household waste.

Built as my project for the **1M1B Green Internship** (Data Analytics & Sustainability track, in partnership with AICTE and Salesforce).

**Live site:** https://ecotrace-bangalore.netlify.app/
**Tableau dashboard:** https://public.tableau.com/app/profile/anuska.ghosh2663/viz/Book1_17735688302400/Dashboard1

## What it does

- **Hotspot map:** an interactive Leaflet map of 20 waste hotspots across Bangalore, colour-coded by status (active, reported, under review). Click a marker for details.
- **Recycling centres:** a searchable table of BBMP dry waste collection centres with a zone filter (North, South, East, West, Central), showing ward, address, timings and contact.
- **Waste guide:** segregation guidelines for wet, dry, hazardous and e-waste, plus five practical tips to reduce household waste.
- **Report form:** a form for describing a waste dumping spot (location, zone, issue type, optional photo).
- **Contact section:** BBMP and authority contact details.

## The data work behind it

- Collected, cleaned and structured the BBMP solid waste dataset (336 dry waste collection centres with GPS coordinates) in Google Sheets, handling missing values and standardising zone names.
- Cross-referenced 4 data sources to compile 20+ verified waste hotspots.
- Published a Tableau Public dashboard with 4 visualisations covering zone-wise waste volume and geographic mapping.
- Ran 2 rounds of stakeholder research with 29 respondents.

Data source: [data.opencity.in](https://data.opencity.in), BBMP Solid Waste Management dataset.

## Built with

- HTML, CSS and JavaScript (a single `index.html`, no build step)
- [Leaflet](https://leafletjs.com/) with OpenStreetMap tiles for the map
- Google Sheets (data cleaning) and Tableau Public (dashboard)
- Netlify (hosting)

## Run it locally

No installation is needed.

1. Clone the repository:
   ```bash
   git clone https://github.com/anuskaGHS/EcoTrace.git
   ```
2. Open `index.html` in any browser. An internet connection is needed for the map tiles and fonts.

## Project structure

```
EcoTrace/
├── index.html   # the whole site: layout, styles, map and table logic
├── LICENSE      # MIT
└── README.md
```

## Current limitations

- The centres table on the website shows a selection of centres. The full 336-centre dataset was used in the Google Sheets and Tableau analysis.
- The report form is a front-end demo. It validates the fields and shows a confirmation message, but submissions are not stored or sent to BBMP.

## Possible next steps

- Connect the report form to a backend or form service so reports are actually stored.
- Load the full 336-centre dataset into the site and add a "nearest centre" search.
- Add screenshots to this README.

## Author

**Anuska Ghosh**, BCA (AI & ML), Alliance University, Bangalore
[Portfolio](https://anuskaghosh.netlify.app/) · [LinkedIn](https://www.linkedin.com/in/anuska-ghosh-68ba34318/) · [GitHub](https://github.com/anuskaGHS)

## License

Released under the [MIT License](LICENSE).
