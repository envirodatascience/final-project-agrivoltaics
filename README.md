[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/g_e38bz1)
1) Define the Questions & Goals of the Project

Agrivoltaics, also known as solar sharing, is the co-developing of the same area of land for both solar photovoltaic power generation and agriculture. It involves installing solar panels at a higher elevation with wider spacing, allowing crops to be grown underneath and between the panel arrays. As such, agrivoltaics can be a non-invasive, but instead additive way for clean energy generation.

Key benefits of agrivoltaic systems include:

- Increased land productivity by generating solar electricity and crops simultaneously on the same land
  
-   According to the Aspen Institute, carbon dioxide and water use efficiency both increase significantly with agrivoltaics, suggesting that the reduction of stress from heat and drought aid overall productivity

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
- Title in GitHub: TRUE_UK_renewable_energy_location.csv

- Database of Global Administrative Areas (GADM). 2022. “United Kingdom.” https://gadm.org/download_country_v3.html#google_vignette
- Title in GitHub: GBR_3.zip

- Department for Environment, Food, and Rural Affairs. June 2023. “Structure of the agricultural industry in England and the UK at June.” https://www.gov.uk/government/statistical-data-sets/structure-of-the-agricultural-industry-in-england-and-the-uk-at-june
- Title in GitHub: NUMBER_TRUE_UK_regional_ag_2023 - Total_farmed_area.csv

UK Data Notes: 

- UK renewable energy data: UK government data with all UK renewable energy project data as of October 2023. As specific agrivoltaic project data is not available, operational ground-standing solar farm data is used as a proxy. 

- UK shapefile: Database of Global Administrative Areas data used, which provided UK breakdown at the county level. The coordinate reference system is longitude/latitude and the WGS84 datum.

- UK agricultural land use: DEFRA (the UK Department for Environment, Food, and Rural Affairs) only has agricultural census data for land use within England, and at the regional level. It remains conducive for us to work with this data as the South of England is the area with the sunlight hours most conducive to agrivoltaics. We needed to dissolve the county-level boundaries from earlier in order to work with this regional-level data.

- Data for solar duration in the UK was calculated through the Astral package in Python.

India data:

- Visual Aid: Map of India with labeled state names, from Wikipedia

- Title in Github: Map-of-India-States.gif

- Existing Agrivoltaic Sites: Ortiz, A., Negandhi, D., Mysorekar, S.R. et al. Sci Data 9, 497 (2022). “An Artificial Intelligence Dataset for Solar Energy Locations in India”. https://doi.org/10.1038/s41597-022-01499-9

- Title in Github: solar_farms_india_2021_merged_simplified (1) (1).geojson

- Shapefile of India: Public Dataset on Github, published by Anuj Tiwari. https://github.com/AnujTiwari/India-State-and-Country-Shapefile-Updated-Jan-2020

- Title in Github: India-State-and-Country-Shapefile-Updated-Jan-2020

- Energy Access: Shalu Agrawal, Sunil Mani, et al. Council on Energy, Environment, and Water. October 2020. “State of Electricity Access in India.”https://www.ceew.in/sites/default/files/ceew-research-on-state-of-electricty-access-and-coverage-in-india.pdf

- Title in Github: states without electricity.xlsx

- Villages in India by State: Statista. September 2015. “Leading states and union territories with the highest number of villages* in India in 2012. https://www.statista.com/statistics/615731/number-of-villages-by-state-and-union-territory-india/

- Title in Github: statistic_id615731_villages-in-india---by-state-and-union-territory-2012 2 (1).xlsx

- Solar Potential by State: Ministry of New and Renewable Energy (India). November 2022. “Annual Report 2021-22.” https://mnre.gov.in/annual-reports-2021-22/

- Title in Github: [EDITED] Solar Potential.xlsx

- Agriculture by State in India: International Crops Research Institute for the Semi-Arid and Tropics. 2017. http://data.icrisat.org/dld/src/visualization.html

- Title in Github: Agriculture_by_State.csv

- Secondary Agriculture Land: Ministry of Agriculture, Cooperation, and Farmers Welfare. August 2021. “Irrigated Agricultural Land.” https://sansad.in/getFile/loksabhaquestions/annex/176/AU2416.pdf?source=pqals

Data limitations/any major notes:

- Visual Aid: To be used in reference to the data analysis

- Existing Agrivoltaic Sites: This dataset used a combination of satellite imagery, AI, and human verification to map  1363 solar PV farms in India

- Energy Access: These data are presented by the Council on Energy, Environment, and Water based on the 2020 insights from the India Residential Energy Survey

- Shapefile of India: This shapefile, once unzipped, allowed us to map the country of India with state boundaries

- Villages in India by State: These data are drawn from numbers originating in 2012

- Solar Potential by State: These data come from the Annual Report of the Ministry of New and Renewable Energy. However, there are not all of the same states represented here compared to the India state shapefile.

- Agriculture by State in India: This project, called the District Level Database and operated by the International Crops Research Institute for the Semi-Arid Tropics as well as the Tata-Cornell Institute. The website allows a researcher to download data by state, crop, and date range.

- Secondary Agriculture Land: These data were drawn from a figure published by the Government of India. These data were used to supplement the main agriculture dataset in order to fill in the NaN values of those states for which no agricultural data was available in the original dataset. These data are drawn from 2017-2018 data. This dataset is not uploaded into Github because the individual datapoints were input manually into the dataframe.


3) Answer research question

In the UK, agrivoltaics present a number of significant potential benefits including increased energy independence during a time of heightened geopolitical tensions, and a transition to clean renewable energy as the UK seeks to meet its domestic and international climate commitments. The major challenges in the UK will be solar availability, along with land availability - given how much smaller the UK is than India. As seen in our final analysis, the South East region (which includes London) has by far the most solar farms, but less agricultural land. This is logical given the propensity of urban solar projects, and the urban zoning of much of the land in this area.

Excluding the South East, the South West and East Midlands regions have the most solar farms, and the South West has the most agricultural land available, and also as the southern-most region, has the greatest sunlight hours during the shortest days of the year. As such, we would recommend that the UK government continue to investigate other factors such as agricultural land type (agrivoltaics may be best suited in an are mostly used for livestock grazing), and farmer environmental and energy sentiment to further evaluate which counties within the South West region of England would grant an agrivoltaics pilot project the greatest likelihood of success. 

In India, numerous factors influence the situation of agrivoltaics. According the the Rockefeller Institute, while great strides have been made, 304 million people in India still lack access to electricity. Agrivoltaics can be installed on pre existing farmland, requiring no additional land to bring renewable energy to crops. As a result, agrivoltaics can address the dual crises in India of energy security and renewable energy.

As the most populous nation in the world, India has a great impact on the global emissions levels. In order to maintain the goal of keeping warming below the 1.5 pre-industrial level, all nations will need to transition to a heavy reliance on renewable energy. For their compact nature and their ability to coexist with farmland, agrivoltaics are a vital tool in that transformation.

According to our analysis, a viable state in which to increase agrivoltaic installed capacity is Rajasthan. This state has the highest level of solar potential as well as a very high level of agricultural land coverage. The result is the prime condition for increased agrivoltaic deployment. 

Another viable state for agrivoltaics would be Uttar Pradesh, the state with the highest amount of villages lacking electricity in India (7261). Agrivoltaics installed on its ample farmland (24165 thousand ha) would greatly alleviate the energy access issues in that state.

As our analysis indicates, India and the UK are very different geographical contexts and stand to reap different benefits from an agrivoltaics implementation that are relevant to their national needs. However, this project emphasizes that similar social, industrial, and physical factors will influence the success of any agrivoltaics program: where is there enough sun, where is there enough farmland, and where are the commercial, legal, and social variables aligned for implementation? Our project directs the governments of the UK and India into a refined geographic search for the best site for a national pilot project, but also lays the foundation for a global modeling system that could be used to suggest the factors to consider before setting up an agrivoltaics program in any area around the world.

Instructions to view code:
- Code and analysis are in 617_Agrivoltaics_India and 617_Agrivoltaics_UK. The notebooks can be read in any order. The UK notebook can be opened directly from GitHub using the Colab link. To open the larger India notebook:
1) Open Colab
2) Select Github
3) Select envirodatascience/final-project-agrivoltaics, then select 617_Agrivoltaics_India.ipynb

