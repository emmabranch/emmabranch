# Hi, I'm Emma Branch 👋

I'm an epidemiologist and population health researcher, and a PhD candidate in epidemiology at the University of British Columbia. My research looks at wildfire smoke exposure and perinatal and infant health. I like turning complex data into clear evidence that public health teams, planners, and communities can act on. Lately I've been applying the same skills to ocean and fisheries data, with a focus on documented, reproducible workflows.

**Interests:** environmental and climate health, ocean and fisheries data, health equity, spatial epidemiology, and knowledge translation.

## Portfolio projects

### 🎣 BC fish stock status: an exploratory rapid assessment toolkit
What do public data actually tell us about the status of BC's fish and shellfish stocks, and where do they run out? I combined DFO's 2024 Sustainability Survey for Fisheries with the RAM Legacy Stock Assessment Database to build a documented database for ten stocks across six species, including five Pacific herring areas. Each stock gets a data tier, a biomass-to-limit-reference-point indicator, and rule-based data gap flags, and a parameterised Quarto template renders a two-page summary for any stock. The latest estimates were consistent with all seven DFO 2024 status zones that could be compared. Only two of the ten stocks had both biomass and fishing-pressure ratios relative to MSY, and two relied on DFO's survey response alone. This is a learning project, not an official assessment.
- **Tools:** R (tidyverse, leaflet, plotly, patchwork), Quarto (Typst PDF reports, closeread scrollytelling), GitHub Pages
- [Project site and interactive map](https://emmabranch.github.io/bc-fish-stock-status/) | [Stock cards](https://emmabranch.github.io/bc-fish-stock-status/cards.html) | [Code](https://github.com/emmabranch/bc-fish-stock-status)

### 🌊 BC lightstation sea temperatures: quality control and the 2014 to 2016 marine heatwave
How do you turn decades of hand-collected ocean temperatures into data others can trust and reuse? I took daily sea surface temperatures from 12 BC lightstations (about 140,000 observations since 1991) from CIOOS Pacific's ERDDAP server and applied automated quality control based on the IOOS QARTOD manuals, tuning each test to the data and documenting every decision. About 1% of values were flagged, and the checks turned up periods of whole-degree recording at several stations. The cleaned data are published as a CF and ACDD compliant NetCDF file with a data dictionary and archived with a DOI. Maps and a heatmap show the 2014 to 2016 marine heatwave reaching the BC coast.
- **Tools:** R (rerddap, ncdf4, sf, leaflet, gganimate), Quarto, IOOS Compliance Checker, Zenodo
- [Project site and interactive map](https://emmabranch.github.io/bc-lightstation-qc/) | [Code](https://github.com/emmabranch/bc-lightstation-qc) | [DOI: 10.5281/zenodo.24326157](https://doi.org/10.5281/zenodo.24326157)

### 🔥 BC wildfire history in BigQuery
Is British Columbia seeing more wildfires, or just bigger ones? I loaded 75 years of BC Wildfire Service records (about 225,000 fire points and perimeters, 1950 to 2025) into Google BigQuery and analysed them with SQL and BigQuery GIS. The number of fires each year hasn't increased, but area burned has soared: from 2020 to 2025, an average of 1.1 million hectares burned each year, around ten times the average in earlier decades. A spatial query shows how much land has burned within 50 km of five BC communities, decade by decade.
- **Tools:** Google BigQuery, BigQuery GIS, SQL, R (bcdata, sf, bigrquery, ggplot2)
- [Code and findings](https://github.com/emmabranch/bc-wildfire-bigquery)

### 🌡️ Climate resilience and equity profile of VCH communities
Which communities in the Vancouver Coastal Health region are most socially vulnerable to extreme heat and wildfire smoke, and do they also have less green cover? I built a transparent social vulnerability index from 2021 Census data, validated it against Statistics Canada's Canadian Index of Social Vulnerability, mapped it alongside vegetation cover, and wrote a two-page briefing for Medical Health Officers and planners.
- **Tools:** R, sf, leaflet, Quarto, GitHub Pages
- [Interactive map](https://emmabranch.github.io/vch-climate-equity-profile/) | [Briefing note](https://emmabranch.github.io/vch-climate-equity-profile/briefing.html) | [Code](https://github.com/emmabranch/vch-climate-equity-profile)

### 🐟 BC Salmon Explorer
How are BC's wild salmon doing? This interactive R Shiny app maps nearly 7,000 spawning streams from the Fraser to the Yukon. You can filter by species, region, and Conservation Unit, then see which
