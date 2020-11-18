# Stat199-Final-Project

Alexis Bianco, Pierce Hollier, Hadeel Hamoud, Ryan Lee

The primary goal in this project is to understand the correlation between climate change indicators 
and the refugee flow from at-risk countries. In order to make the analysis more manageable, we focused 
on the climate change and refugee data of the Middle East region.

----------------------------------------VARIABLES UTILIZED----------------------------------------

Time: year of data records.

Country Name: the name of each country in the region of interest.

arable_land: percent of land in each country that is arable. Further represented by the dataframe 
climate_arable.

land_cereal: hectares of land under cereal production in each country. Further represented by the dataframe
climate_cereal.

co2_tons: CO2 emissions in metric tons per capita in each country. Further represented by the dataframe
climate_co2.

nitrous_tons: Nitrous oxide emissions in thousand metric tons of CO2 equivalent per country. Further
represeted by the datafhrame climate_nitrous.

nitrous_kt_per_capita: Nitrous oxide emissions in thousand metric tons of CO2 equivalent per capita per
country.

methane_tons: Methane emissions in energy sector in thousand metric tons of CO2 equivalent per country. 
Further represented by the dataframe climate_methane.

methane_kt_per_capita: Methane emissions in energy sector in thousand metric tons of CO2 equivalent per 
capita per country. 

refugee: number of refugees recorded in each country for each year. Further represented by the dataframe
climate_refugee.

pop: overall population of each country for each year.

prop_refugee: proportion of refugees (refugee / population) calculated each year for each country.

refugee_per_100000: number of refugees per 10,000 residents.

----------------------------------------DATAFRAMES----------------------------------------

climate: a condensed dataframe containing the variables Time, Country Name, arable_land, land_cereal, 
co2_tons, nitrous_tons, nitrous_kt_per_capita, methane_tons, methane_kt_per_capita, refugee, pop, and prop_refugee.

climate_data: a condensed dataframe containing the variables Time, Country Name, arable_land, land_cereal, 
co2_tons, nitrous_tons, nitrous_kt_per_capita, methane_tons, methane_kt_per_capita, refugee, pop, and prop_refugee. 
Filtered to only inlcude the countries Afghanistan / Iran, Islamic Rep. / Iraq / Pakistan / Syria.

climate_filtered: a version of climate_data with the rows containing N/A values filtered out.

climate_me: a condensed dataframe containing the variables Time, Country Name, arable_land, land_cereal, 
co2_tons, nitrous_tons, nitrous_kt_per_capita, methane_tons, methane_kt_per_capita, refugee, pop, and prop_refugee. 
Filtered to only inlcude the countries Afghanistan / Iran, Islamic Rep. / Iraq / Pakistan.

climate_sahel: a condensed dataframe containing the variables Time, Country Name, arable_land, land_cereal, 
co2_tons, nitrous_tons, nitrous_kt_per_capita, methane_tons, methane_kt_per_capita, refugee, pop, and prop_refugee. 
Filtered to only inlcude the countries Afghanistan / Iran, Islamic Rep. / Iraq / Pakistan

----------------------------------------LINEAR MODELS----------------------------------------

climate_model: a linear model with a logarithmic transformation used to estimate predicted refugee 
proportion of population in a particular country based off cereal land, CO2 emissions, nitrous emissions, 
and methane emissions. Only includes major effects. 

climate_model_aug: augmented version of climate_model.

climate_filtered_sahel: a condensed dataframe fitted for the Sahel region, containing the variables 
Time, Country Name, arable_land, land_cereal, co2_tons, nitrous_tons, nitrous_kt_per_capita, methane_tons,
methane_kt_per_capita, refugee, pop, and prop_refugee. Filtered to only inlcude the countries Afghanistan / 
Iran, Islamic Rep. / Iraq / Pakistan. Rows containing N/A values were also filtered out.

climate_interac: a linear model with a logarithmic transformation used to estimate predicted refugee 
proportion of population in a particular country based off of cereal land, CO2 emissions, nitrous emissions, 
and methane emissions. Includes major effects and greenhouse gas interactions. 

climate_int_aug: augmented version of climate_interac.

----------------------------------------PREDICTED VALUE DATAFRAMES----------------------------------------

predicted_afghan: a condensed dataframe containing the variables Time, Country Name, arable_land, land_cereal, 
co2_tons, nitrous_tons, nitrous_kt_per_capita, methane_tons, methane_kt_per_capita, refugee, pop, and prop_refugee. 
Filtered to only inlcude the country Afghanistan.

predicted_iran: a condensed dataframe containing the variables Time, Country Name, arable_land, land_cereal, 
co2_tons, nitrous_tons, nitrous_kt_per_capita, methane_tons, methane_kt_per_capita, refugee, pop, and prop_refugee. 
Filtered to only inlcude the country Iran, Islamic Rep. 

predicted_iraq: a condensed dataframe containing the variables Time, Country Name, arable_land, land_cereal, 
co2_tons, nitrous_tons, nitrous_kt_per_capita, methane_tons, methane_kt_per_capita, refugee, pop, and prop_refugee. 
Filtered to only inlcude the country Iraq.

predicted_pak: a condensed dataframe containing the variables Time, Country Name, arable_land, land_cereal, 
co2_tons, nitrous_tons, nitrous_kt_per_capita, methane_tons, methane_kt_per_capita, refugee, pop, and prop_refugee. 
Filtered to only inlcude the country Pakistan.

predicted_values: a condensed dataframe containing the variables Time, Country Name, arable_land, land_cereal, 
co2_tons, nitrous_tons, nitrous_kt_per_capita, methane_tons, methane_kt_per_capita, refugee, pop, and prop_refugee. 
Filtered to only inlcude the country Burkina Faso.

