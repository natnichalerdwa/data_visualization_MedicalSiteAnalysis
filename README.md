# Los Angeles Medical Site Analysis

The purpose of this analysis was to explore the cities within Los Angeles County that would be suitable for a medical facility. This analysis has successfully satisfied its purposes. The candidate cities were clustered, and the most common venues around each of those cities were identified through Foursquare API. However, since there are many factors that contribute to the success potentials of a big project like a medical facility, such as risk factors and target patients, the investor would have to consult many other specialists before deciding on the most suitable city for his/her facility.

## Data
* The Json file of L.A. county's spatial data was published by Los Angeles Times. The coordinates of L.A. was found through Google Maps API Geocoding. The coordinates would be used to plot a folium map
* The CSV file containing a comprehensive list of cities in the US and their coordinates was retrieved from Simplemaps. The file was cleaned up to extract data of cities within L.A. County
* The list of healthcare facilities in L.A. county is retrieved from California Hospital Association. Although the list shows all hospitals in California, when visualizing with a choropleth map, only the cities in L.A. gets filled, as the json file only contains L.A. county boundary map
* The top venues in each candidate city were found through Foursquare API. The venues were clustered, and a cluster map was generated

## Methodology
* To illustrate the data, a choropleth map was generated (the coordinates of L.A. was retrieved from Google Maps API). The map displays an abundance of medical facilities by shading areas where at least one medical facility exists.
* The Foursquare API was accessed to retrieve the list of all nearby venues to the candidate cities. A total of 1,426 venues were returned. Then, the top 10 venue categories in each candidate city was retrieved.
* An ideal location for a medical facility should be in proximity to restaurants and cafes to ensure maximum comfort for patients and caretakers. The candidate cities were clustered into 3 clusters using K-Means Clustering.
* A cluster map displaying markers of cities from each cluster was generated to visualize the results.
