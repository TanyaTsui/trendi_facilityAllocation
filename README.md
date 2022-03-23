# trendi_facilityAllocation
This repo contains the jupyter notebooks required to conduct a facility allocation analysis for the food upcycling startup Trendi. Using k-means clustering and agricultural data, we estimate the optimal number and location of Trendi machines and facilities in Canada. 

The analysis process consists of three steps, separated into three notebooks: 
* Data wrangling 1 - Converting raster data on crop locations (from the Annual Crop Inventory) to a shapefile with points, categorizing points into the correct provinces. This is done in the notebook `01_dataWrangling_1_cropProvinces_simple.ipynb` 
* Data wrangling 2 - Estimating the waste yield at each point location in Canada, using per province crop yield data from Statistics Canada. This is done in the notebook `01_dataWrangling_2_calcYield_dummy.ipynb`  
* Spatial analysis - Identifying optimal number and location of Trendi machines and facilities using k-means clustering analysis. This is done in the notebook `02_kMeansConstrained_canada.ipynb` 
