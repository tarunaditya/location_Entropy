# location_Entropy
generic module that generates location entropy based on location visits distributed across time &amp; can be modified to do the same for visits distributed across users if the input data is available in that format


#read data from https://data.cityofchicago.org/Education/Libraries-2011-Visitors-by-Location/xxwy-zyzu
# googled this data in https://toolbox.google.com/datasetsearch
# Note that in this data set the visit distribution is temporal (across months)
# the same process can be replicated if visit distribution is across users


# few basic preprocessing
# 1. to replace NaN with0
# 2. add a place identifier


the notebook also includes unit test
# Unit test

# subsequent code is just an inference & common sensical check that serves as unit test
# we start with an intuition that entropy might be low for parks & high if place is not like park & more like street
# used to check if the entropy is atleast dissimilar 
# But we dont have places categorization, so we look at if we are able to tag places & derive it from the place description
