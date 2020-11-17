# Stat199-Final-Project

Alexis Bianco, Pierce Hollier, Hadeel Hamoud, Ryan Lee

The primary goal in this project is to understand the correlation between climate change indicators 
and the refugee flow from at-risk countries. In order to make the analysis more manageable, we focused 
on the climate change and refugee data of the Middle East region.

climate: a condensed dataframe containing the variables Time, Country Name, arable_land, land_cereal, 
co2_tons, nitrous_tons, methane_tons, refugee, pop, and prop_refugee.

climate_model: a linear model with a logarithmic transformation used to estimate predicted refugee 
proportion of population in a particular country based off arable land, cereal land, CO2 emissions, 
nitrous emissions, and methane emissions. (The augmented version is listed under climate_model_aug).

Time: year of data records.

Country Name: the name of each country in the region of interest.

arable_land: percent of land in each country that is arable. Further represented by the dataframe 
climate-arable.

land_cereal: hectares of land under cereal production in each country. Further represented by the dataframe
climate_cereal.

co2_tons: CO2 emissions in metric tons per capita in each country. Further represented by the dataframe
climate_co2.

nitrous_tons: Nitrous oxide emissions in thousand metric tons of CO2 equivalent per country. Further
represeted by the datafhrame climate_nitrous.

methane_tons: Methane emissions in energy sector in thousand metric tons of CO2 equivalent per country. 
Further represented by the dataframe climate_methane.

refugee: number of refugees recorded in each country for each year. Further represented by the dataframe
climate_refugee.

pop: overall population of each country for each year.

prop_refugee: proportion of refugees (refugee / population) calculated each year for each country.

