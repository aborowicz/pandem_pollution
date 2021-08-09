Read me for pandem_pollution

In this project I walk through an approach to looking at the question of whether the COVID shutdown in New York City had a measurable effect on air quality. In particular, I'll look at 3 common pollutants - Carbon monoxide, Nitrogen dioxide, and fine particulate matter (PM 2.5) as recorded by EPA air quality monitoring stations.

Opening the R project (```pandem_pollution.Rproj```) will be the easiest way to work with these data and to review the analysis.

The Project includes an R Markdown document (```Pandem_AirQUal.Rmd```) which, when run, will knit the html document included herein (```Pandem_AirQual.html```).

The data used here come from the Environmental Protection Agency in the United States, and are independently avaiable at https://www.epa.gov/outdoor-air-quality-data/download-daily-data

I have collected the relevant data in the ```./data/``` folder. They are stored as csv files, where each csv is the collected data for a particular pollutant in a particular year. In this case I have used PM 2.5, Carbon monoxide, and NO2. Other pollutants are available via the EPA.

At one stage of the analysis, I use a JAGS model. This model is stored as a ```.jags``` file (```Pollutants_NYC.jags```) and is called directly in the RMD file. 