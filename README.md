# Data science for real estate
## Built Heritage vs Real Estate Market. The Barcelona case 
Data science project in Python </br>
tools: Jupyter Notebook, Python,  Idealista API  +  Pandas +  Geopandas +  Numpy +  Folium + BeautifulSoup + OSMNX + Matplotlib + Plotly + Networks + PyTorch + Mapbox API.
## Questions
- How official status of built heritage affects real estate prices?
- How correlation could be identified geographically?
- What is the difference between correlations of oficially listed built heritage or old buildings over 50 years with real estate prices?
## What I learned: 
- Idealista API for query of real estate lots
- Geographical distribution of data by natural jenks
- Spatial lag

## Key takeaways
- spatial affect of built heritage spreads within isochrones of 10-munites walk from listed buildings
- festivals in Spain have categories that correlate with state and local subventions: Interes Internacional, Interes National, Interes Local
- main concentration of festivals is allocated in Catalan Countries: Catalonia, Valencia, Balearic Islands, and Galicia

## video presentation
[![](https://img.youtube.com/vi/d7XqRdQ6O6Y/2.jpg)](https://www.youtube.com/watch?v=d7XqRdQ6O6Y)
## methodology
1. Evaluate the best way of creating a real estate prices dataset by testing API and scraping approaches, finally get a dataset with sufficient data entries. [source>>](DS3_FIN_11.ipynb)
2. Calculate the price per sqm for each data entry in the real estate prices dataset.
3. Match the real estate prices dataset with the Barcelona neighborhood shapefile, calculate mean, max, min, and average price per sqm.
4. Fetch heritage points and polygons from OpenStreetMap, create isochrones of them at 100, 400, and 800 meters.
5. Fetch buildings data from the public cadastre, categorize them by heritage-like and not (already 50 years old buildings could fit the built heritage policy requirements), cluster buildings, make buffers of 400m, match the amount of heritage-like buildings with the Barcelona neighborhood shapefile.
6. Make a correlation between mean, max, min, and average price per sqm and heritage buffer zones, heritage-like buffer zones.
7. Evaluate the hypothesis, check the data on conditions of heritage buildings in non-correlated zones.
## data visualization
### Spinning Globe with datalabels of hemp production by country
![Alt text](visuals/globe_fin.gif)
### Grasshopper definition of Global hemp production
![](visuals/globe001.png)

## References
- OpenStreetMap: [OpenStreetMap](https://www.openstreetmap.org)
- Institut Cartogràfic i Geològic de Catalunya: [ICGC](http://www.icgc.cat)
- Public Cadastre of Spain: [Cadastre](https://www.sedecatastro.gob.es/)
- Idealista.es – Spain's #1 Real Estate Web Portal: [Idealista](https://www.idealista.es)
- Fotocasa.es – Spain's #2 Real Estate Web Portal: [Fotocasa](https://www.fotocasa.es)
