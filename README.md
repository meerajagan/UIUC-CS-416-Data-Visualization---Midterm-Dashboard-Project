# cs416_midtermDashboardproject

**Data Pulls**

Volcano Data Pulled from: https://www.kaggle.com/datasets/jessemostipak/volcano-eruptions

According to the provenence, the Volcano Data is originally pulled from this [Github link](https://github.com/rfordatascience/tidytuesday/blob/master/data/2020/2020-05-12/readme.md) and originates from [The Smithsonian Institution]( https://volcano.si.edu/). The only files used for this dashboard were the files "volcanoes" and "eruptions"

Tectonic plate information came from this [website]([url](https://nordpil.com/resources/tectonic-plates-gis-data/index.html)) with a [Github link]([url](https://github.com/fraxen/tectonicplates)) attached at the bottom.

**Data Cleaning and Preprocessing**

The data was cleaned once over using Alteryx and the flows can be found in the "Alteryx Flows Folder". This was primarily to fix any type issues that may have appeared in the data. Furthermore, a tectonic plate mapping was conducted to give better insight into the data when creating the Tableau Dashboard. For this, the data from the "eruptions" file were spatially mapped alongside the publicly available tectonic plate SHP files. 

**What are the Files in this Repo used for dashboarding**

* 'eruptions_fixed_types' - the eruptions fixed data sheet. This is the sheet we will use as a root to make sure we are only looking at volcanoes that have known eruptions.
* 'eruption_plate_mapping' - this sheet maps the eruption centroids (lat/long coords) to its corresponding tectonic plate.
* 'volcanoes_fixed_types'  - the type fixed volcano data sheet. This sheet will give us extra information about each of the volcanoes with eruptions.

**Alteryx Files**

* 'cleaningeruptiondata.yxmd' - Alteryx flow to clean the eruption data sheet
* 'cleaningvolcanodata.yxmd' - Alteryx flow to clean volcano data sheet
* 'volcano_plateMapping.yxmd' - Alteryx flow to spatially map eruption data to tectonic plate data

**Extra Images**

Some extra images used for dashboarding. Images from Google Images.


**How Files were joined in Tableau**

Eruption and Volcano were left joined.

<img width="667" alt="joins" src="https://github.com/meerajagan/cs416_midtermDashboardproject/assets/79546477/4af4fc18-90bb-49b8-9cd6-60f7db287e33">

