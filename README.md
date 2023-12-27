# Geospatial-Visualization-with-Folium
Create interactive maps with markers using the Folium library.
import folium

# Assume you have latitude and longitude coordinates
location = [37.7749, -122.4194]

# Create a folium map centered at the location
my_map = folium.Map(location=location, zoom_start=12)

# Add a marker to the map
folium.Marker(location=location, popup='Your Marker Popup').add_to(my_map)

# Save the map to an HTML file
my_map.save('map.html')
