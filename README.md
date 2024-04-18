# Project 3 - Data Visualization

## About The Project
**Overview and Purpose:** For our project, we explored the patterns in registered vehicle types and gas prices in California from 2019-2023. We examined the relationships between gas prices and electric/hybrid vehichles, the rate at which electric/hybrid vehicles have grown compared to gas powered counterparts, and how the growth of electric/hybrid vehicles have affected the number of charging stations in California. 

The Jupyter Notebooks are broken into two files.  The file titled 'project3_database' shows the process in how we cleaned the data and loaded it into a PostgreSQL database. The second file titled 'project3_visualizations' shows all the transformations and visualizations created to analyze the data. 

## Getting Started
**Usage:** To successfully display all the visualizations in this notebook, ensure that these Python libraries are installed.
- Folium
```bash
pip install folium
```
- GeoPandas
```bash
pip install geopandas
```
**Instructions:** Under the "Fuel Types" heading of the 'project3_visualizations' notebook, the second visualization has a bar chart displaying Count of Vehicles By Fuel Type with a dropdown menu.  Change the dropdown menu from 2019-2023 to show the different vehicle counts by fuel type by year.  

The original dataset provided several fuel types, but we grouped them as shown below:
- Gasoline - Gasoline, Flex-Fuel, Natural Gas
- Hybrid - Hybrid Gasoline, Plug-in Hybrid
- Hydrogen - Hydrogen Fuel Cell
- Electric - Battery Electric
- Diesel - Diesel and Diesel Hybrid

The last visualization under the "Electric Chargers in CA" heading of the same notebook is a choropleth map of the total number of electric chargers in each California county from 2020-2023.  There is a dropdown menu that will show the different choropleth maps for each year and hovering over any county will bring up tooltips that display the county name and the total number of chargers for that year. There is also a layer control button on the top right that allows the user to toggle on/off the choropleth map overlay. 

The choropleth map is displayed by log scale to normalize the dataset, however the tooltip will display the actual number of electric chargers. 


## Ethical Considerations
When considering the datasets concerning California gas prices (all grades and premium),  EV charging stations, and the registration numbers of different vehicle types based on fuel sources, the team considered some ethical implicates. It's important to recognize the implications surrounding lithium mining for battery vehicles, California tax credits incentivizing EV adoption, oil extraction practices, and environmental degradation. Our analysis and visualizations could be used to help acknowledge the ethical dilemmas inherent in promoting electric vehicles while potentially exacerbating environmental harm through lithium mining. The data and analysis could also bring about topics of maintaining a balance between encouraging sustainable practices and minimizing adverse impacts on ecosystems and communities within California. Additionally, this analysis could help understand the socioeconomic disparities in accessing EV infrastructure and the implications of tax credits on income inequality adds different layers of ethical complexity to the data analysis process.

## References
**Data Sources:** We sourced vehicle fuel type data from ca.gov and gas/diesel price data from the U.S Energy Information Administration.  The electric charger dataset was gathered from kaggle.com
- [CA Vehicle Fuel Types](https://data.ca.gov/dataset/vehicle-fuel-type-count-by-zip-code)
- [CA Gas and Diesel Prices](https://www.eia.gov/dnav/pet/pet_pri_gnd_dcus_sca_a.htm)
- [CA Electric Chargers](https://www.kaggle.com/datasets/natalyamatyushenko/electric-chargers-ca)

**Resources Used:** To help create our visualizations we referred to following:
- [Seaborn Documentation](https://seaborn.pydata.org/examples/errorband_lineplots.html)
- [Pandas Documentation](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.unstack.html)
- [Jupyter Widgets Documentation](https://ipywidgets.readthedocs.io/en/latest/examples/Widget%20List.html)
- [Folium Documentation](https://python-visualization.github.io/folium/latest/user_guide/geojson/geojson_popup_and_tooltip.html)
- [GeoPandas Documentation](https://geopandas.org/en/stable/docs/user_guide/io.html)
- [Geeks for Geeks](https://www.geeksforgeeks.org/grids-in-matplotlib/)
- XPERT Learning Assistant

### Group Members:
- Amar Khokhar
- Bianca Sabino
- Chung-Ting Liao
- Santos Marquez
