[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/g_e38bz1)
1) Define the Questions & Goals of the Project

Agrivoltaics, also known as solar sharing, is the co-developing of the same area of land for both solar photovoltaic power generation and agriculture. It involves installing solar panels at a higher elevation with wider spacing, allowing crops to be grown underneath and between the panel arrays. As such, agrivoltaics can be a non-invasive, but instead additive way for clean energy generation.

Key benefits of agrivoltaic systems include:

- Increased land productivity by generating solar electricity and crops simultaneously on the same land

- Potential for higher crop yields due to the sheltering effect of the solar panels

- Water conservation as the panels help reduce evaporation from the soil and plants

- Improved solar panel efficiency as the evaporation from the plants helps cool the panels

- Diversified income streams for farmers from selling both crops and solar electricity

In this project, we have selected two geographical contexts, India and the UK. Linked by their colonial heritage, the two nations today face very different geographical sizes and conditions, populations, and energy needs. The UK has widespread energy access, but is seeking ways to transition to clean and independent energy sources. India has less widespread access to energy and so innovative solutions that could also support agricultural projects would have significant humanitarian benefits. We are interested in comparing how a similar solution could yield results beneficial to these two different nations. 

These factors include:

- Where existing solar farms or agrivoltaic programs exist (which indicates the presence of factors suitable for commercial success)

- Where the sunlight hours in each nation meet the requirements for commercial operation

- Where the greatest amount of agricultural land is available in each nation

We will combine the above to suggest the region in each nation that merits further investigation into a pilot project.

2) Source Data

UK data:

- Department for Energy Security and Net Zero. October 2023. “Renewable Energy Planning Database”. https://researchbriefings.files.parliament.uk/documents/CBP-7434/CBP-7434.pdf

- Database of Global Administrative Areas (GADM). 2022. “United Kingdom.” https://gadm.org/download_country_v3.html#google_vignette 

- Department for Environment, Food, and Rural Affairs. June 2023. “Structure of the agricultural industry in England and the UK at June.” https://www.gov.uk/government/statistical-data-sets/structure-of-the-agricultural-industry-in-england-and-the-uk-at-june 

Data notes: 

- UK renewable energy data: UK government data with all UK renewable energy project data as of October 2023. As specific agrivoltaic project data is not available, operational ground-standing solar farm data is used as a proxy. 

- UK shapefile: Database of Global Administrative Areas data used, which provided UK breakdown at the county level. The coordinate reference system is longitude/latitude and the WGS84 datum.

- UK agricultural land use: DEFRA (the UK Department for Environment, Food, and Rural Affairs) only has agricultural census data for land use within England, and at the regional level. It remains conducive for us to work with this data as the South of England is the area with the sunlight hours most conducive to agrivoltaics. We needed to dissolve the county-level boundaries from earlier in order to work with this regional-level data.

- Data for solar duration in the UK was calculated through the Astral package in Python.

3) Answer research question

In the UK, agrivoltaics present a number of significant potential benefits including increased energy independence during a time of heightened geopolitical tensions, and a transition to clean renewable energy as the UK seeks to meet its domestic and international climate commitments. The major challenges in the UK will be solar availability, along with land availability - given how much smaller the UK is than India. As seen in our final analysis, the South East region (which includes London) has by far the most solar farms, but less agricultural land. This is logical given the propensity of urban solar projects, and the urban zoning of much of the land in this area.

Excluding the South East, the South West and East Midlands regions have the most solar farms, and the South West has the most agricultural land available, and also as the southern-most region, has the greatest sunlight hours during the shortest days of the year. As such, we would recommend that the UK government continue to investigate other factors such as agricultural land type (agrivoltaics may be best suited in an are mostly used for livestock grazing), and farmer environmental and energy sentiment to further evaluate which counties within the South West region of England would grant an agrivoltaics pilot project the greatest likelihood of success. 

As our analysis indicates, India and the UK are very different geographical contexts and stand to reap different benefits from an agrivoltaics implementation that are relevant to their national needs. However, this project emphasizes that similar social, industrial, and physical factors will influence the success of any agrivoltaics program: where is there enough sun, where is there enough farmland, and where are the commercial, legal, and social variables aligned for implementation? Our project directs the governments of the UK and India into a refined geographic search for the best site for a national pilot project, but also lays the foundation for a global modeling system that could be used to suggest the factors to consider before setting up an agrivoltaics program in any area around the world.

