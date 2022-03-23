# trendi_facilityAllocation
This repo contains the jupyter notebooks required to conduct a facility allocation analysis for the food upcycling startup Trendi. Using k-means clustering and agricultural data, we estimate the optimal number and location of Trendi machines and facilities in Canada. 

The analysis process consists of three steps, separated into three notebooks: 
* Data wrangling 1 - Converting raster data on crop locations (from the Annual Crop Inventory) to a shapefile with points, categorizing points into the correct provinces. This is done in the notebook `01_dataWrangling_1_cropProvinces_simple.ipynb` 
* Data wrangling 2 - Estimating the waste yield at each point location in Canada, using per province crop yield data from Statistics Canada. This is done in the notebook `01_dataWrangling_2_calcYield_dummy.ipynb`  
* Spatial analysis - Identifying optimal number and location of Trendi machines and facilities using k-means clustering analysis. This is done in the notebook `02_kMeansConstrained_canada.ipynb` 

## Limitations and further work
At this moment (23 Mar 2022), the analysis results are meaningless, because we are missing two essential steps (that will be completed by Arjang): matching statsCan commodity codes to aci codes, and estimating the waste yield for each crop type; which need to be implemented in the second notebook, `01_dataWrangling_2_calcYield_dummy.ipynb`. The results should only be interpreted when the two esstential steps have been taken. 

Additionally, each notebook contains a 'limitations and futher work' section at the end, which shows the steps that need to be taken to further improve the analysis. 
