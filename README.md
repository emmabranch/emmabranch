# Hi, I'm Emma Branch 👋

I'm an epidemiologist and population health researcher, and a PhD candidate in epidemiology at the University of British Columbia. My research looks at wildfire smoke exposure and perinatal and infant health. I like turning complex data into clear evidence that public health teams, planners, and communities can act on. Lately I've been applying the same skills to ocean and fisheries data and to housing indicators, with a focus on documented, reproducible workflows and clear performance reporting.

**Interests:** environmental and climate health, ocean and fisheries data, housing and health equity, performance measurement, spatial epidemiology, and knowledge translation.

## Portfolio projects

### 🏘️ BC municipal housing indicators: a documented performance scorecard
How are the 40 BC municipalities with provincial housing targets doing on supply, need, affordability, and rental vacancy? I built a reproducible R pipeline that combines Statistics Canada Census data, CMHC rental and construction data, and *Housing Supply Act* target results into a tidy indicator database, with an indicator framework that sets out the definition, source, comparator, status rule, and limitations for each of nine indicators. A Quarto dashboard shows red, amber, and green status against targets and BC benchmarks, with an interactive map, and a parameterised template renders a two-page report card for every municipality. Data quality checks caught 6 of 40 incorrect geography codes, the pipeline reproduces Statistics Canada's published BC core housing need rates exactly, and each hand-compiled target value records its source and whether it was verified. 18 of the 30 municipalities assessed so far met their Year 1 housing target. This is a learning project using public data, not affiliated with BC Housing or the Government of BC.
- **Tools:** R (tidyverse, cansim, cmhc, sf, leaflet, reactable), Quarto dashboards and parameterised reports, GitHub Pages
- [Dashboard](https://emmabranch.github.io/bc-housing-indicators/) | [Example report card](https://emmabranch.github.io/bc-housing-indicators/reports/vancouver.html) | [Code](https://github.com/emmabranch/bc-housing-indicators)

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
- [Live site](https://emmabranch.github.io/bc-wildfire-bigquery/) | [Code](https://github.com/emmabranch/bc-wildfire-bigquery)

### 🌡️ Climate resilience and equity profile of VCH communities
Which communities in the Vancouver Coastal Health region are most socially vulnerable to extreme heat and wildfire smoke, and do they also have less green cover? I built a transparent social vulnerability index for 1,773 neighbourhoods from 2021 Census data, validated it against Statistics Canada's Canadian Index of Social Vulnerability (rho = 0.74), and mapped it alongside vegetation cover: the most vulnerable fifth of urban neighbourhoods has about 25% green cover, compared with 35% in the least vulnerable. A two-page briefing for Medical Health Officers and planners draws on VCH's own lived-experience research.
- **Tools:** R, sf, leaflet, Quarto, GitHub Pages
- [Project site](https://emmabranch.github.io/vch-climate-equity-profile/) | [Briefing note](https://emmabranch.github.io/vch-climate-equity-profile/briefing.html) | [Code](https://github.com/emmabranch/vch-climate-equity-profile)

### 🐟 BC Salmon Explorer
How are BC's wild salmon doing? This interactive R Shiny app maps nearly 7,000 spawning streams from the Fraser to the Yukon. You can filter by species, region, and Conservation Unit, then see which populations are declining, holding steady, or recovering, based on mixed-effects models of 30 years of spawner counts.
- **Tools:** R, Shiny
- [Live app](https://emmabranch.shinyapps.io/bc-salmon-explorer) | [Code](https://github.com/emmabranch/bc-salmon-explorer)
- For ocean conditions on the same coast, see [BC lightstation sea temperatures](https://emmabranch.github.io/bc-lightstation-qc/).

### 🦌 Mining claims and caribou ranges in Ontario
How much of Ontario's woodland caribou habitat is staked for mineral exploration? Active mining claims now cover over 50,000 km² of caribou range, nearly the size of Nova Scotia, including almost a third of the Sydney range in the northwest. This project pulls the province's claims data automatically with Python and R, measures the overlap with each range, and maps how staking has shifted since 2018, including a 2025 jump when 60% of newly staked land fell inside caribou range.
- **Tools:** Python, R, QGIS
- [Website](https://emmabranch.github.io/ontario-claims-caribou/) · [Code](https://github.com/emmabranch/ontario-claims-caribou)

## Skills

- **Analysis and programming:** R (tidyverse, sf, Shiny, Quarto, RMarkdown), SAS, SQL, Python, Stata, SPSS
- **Cloud and databases:** Google BigQuery (including BigQuery GIS), bigrquery, REDCap (database design and build)
- **Spatial:** QGIS, ArcGIS, sf, leaflet, BigQuery GIS
- **Performance measurement and reporting:** indicator frameworks, KPI definitions and status rules, scorecards and dashboards (Quarto, Power BI), parameterised reporting, data dictionaries
- **Data management and quality:** data management plans, OCAP principles, quality control (IOOS QARTOD), validation against published figures, metadata standards (CF, ACDD), NetCDF, ERDDAP, data archiving with DOIs (Zenodo), Git and GitHub
- **Methods:** epidemiological study design, environmental exposure assessment, area-level indices, data linkage

## Get in touch

- [LinkedIn](https://www.linkedin.com/in/embranch/)
- emma.branch@gmail.com
