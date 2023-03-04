####################
## Metadata for the datasets associated with:
## Urbanization-driven changes in web-building and body size in an orb-web spider
## Maxime Dahirel, Maarten De Cock, Pieter Vantieghem and Dries Bonte
## Journal of Animal Ecology
## corresponding author: MD: maxime.dahirel [at] yahoo.fr ; https://mdahirel.github.io/ ; Twitter: @mdahirel
####################

there are three datasets:
"individual_spider_info.txt" ; 621 rows; the main dataset with individual trait values
"population_densities_info.txt" ; 62 rows; the secondary dataset with population densities
"landscape_urbanization_info.txt" ; 21 rows; the dataset used to compare landscape-level metrics

###################################################
##(Groups of) Variables present in all three files:
###################################################
"TOWN": name of the town the landscape is located in
"landscape_urba" and "local_urba" (categorical variables, three levels): urbanization levels at the landscape (3*3 km) and local (0.2*0.2 km) scales
"percent_buildings_landscape" and "percent_buildings_site" percentage of a 3*3 km landscape or a 0.2*0.2 km  site occupied by buildings

###########################################################################################
#Variables present in both "individual_spider_info.txt" and "population_densities_info.txt"
###########################################################################################
"PLOT": code identifying each 3*3 km landscape. If dataset compiled without errors, should be redundant with "TOWN"
"Site": code identifying each 0.2*0.2 km site. A version of it can be reconstructed from "TOWN" or "PLOT", "landscape_urba" and "local_urba"
"Date": sampling date, format dd/mm/yyyy
"LAT" and "LON": latitude and longitude of each 0.2*0.2 km site

###########################################################
#Variables present in "population_densities_info.txt" only:
###########################################################
"Naraneus": number of adult female Araneus diadematus spiders caught per 0.2*0.2 km site

########################################################
#Variables present in "individual_spider_info.txt" only:
########################################################
"Id": identifier for each spider
"CTsize": spider cephalothorax width (cm)
"Mesh": average mesh width of the web capture spiral (cm) 
"EfSurface": area of the web capture zone (cm2)
"Eggs": number of mature eggs found inside spiders (only available in some of the individuals)

#############################################################
#Variables present in "landscape_urbanization_info.txt" only:
#############################################################
"CORINE_percent_artificial": percentage of a 3*3 km landscape total area considered artificial based on CORINE land cover (artificial green spaces are excluded from the calculation)