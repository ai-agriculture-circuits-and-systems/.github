# Farmvibes.ai
https://github.com/microsoft/farmvibes-ai

## 1. Automatic Segmentation of BingMaps basemaps
- **Problem:** Segment BingMaps basemaps
- **Goal:** Automatically segment BingMaps basemaps
- **Task:** Use SAM workflow for segmentation
- **Dataset:** BingMaps basemaps

## 2. Automatic Segmentation of Sentinel-2
- **Problem:** Segment Sentinel-2 imagery
- **Goal:** Automatically segment Sentinel-2 imagery
- **Task:** Use SAM workflow for segmentation
- **Dataset:** Sentinel-2 imagery

## 3. Carbon sequestration evaluation with ADMAg and COMET-Farm API
- **Problem:** Derive carbon sequestration information
- **Goal:** Evaluate carbon sequestration with COMET-Farm API
- **Task:** Use ADMAg to retrieve farm data and COMET-Farm API to evaluate sequestration
- **Dataset:** Agricultural fields data from ADMAg

## 4. Crop cycle detection
- **Problem:** Detect crop cycles in a year
- **Goal:** Run time-series analysis to detect crop cycles
- **Task:** Analyze NDVI data to identify crop cycles
- **Dataset:** NDVI data

## 5. Crop land segmentation (1/4) - dataset generation
- **Problem:** Generate a dataset for crop land segmentation
- **Goal:** Create dataset using NDVI and CDL rasters
- **Task:** Generate training dataset for crop land segmentation
- **Dataset:** NDVI and CDL rasters

## 6. Crop land segmentation (2/4) - dataset visualization
- **Problem:** Visualize crop land segmentation dataset
- **Goal:** Explore crop land segmentation dataset visually
- **Task:** Visual exploration of the dataset
- **Dataset:** NDVI and CDL rasters

## 7. Crop land segmentation (3/4) - local model training
- **Problem:** Train a crop land segmentation model
- **Goal:** Train locally a crop land segmentation model
- **Task:** Train the model on local machine
- **Dataset:** Crop land segmentation dataset

## 8. Crop land segmentation (3/4) - model training on Azure Machine Learning
- **Problem:** Train a crop land segmentation model on Azure
- **Goal:** Train crop land segmentation model using Azure Machine Learning
- **Task:** Model training on Azure platform
- **Dataset:** Crop land segmentation dataset

## 9. Crop land segmentation (4/4) - inference
- **Problem:** Infer crop land segmentation for new regions
- **Goal:** Apply trained model to infer segmentation on new regions
- **Task:** Use model to infer crop land segmentation
- **Dataset:** New crop field regions

## 10. Detecting Forest Changes
- **Problem:** Detect changes in forests
- **Goal:** Identify changes in forest areas
- **Task:** Detect forest changes using satellite data
- **Dataset:** Forest area data

## 11. Download ALOS forest extent maps
- **Problem:** Download ALOS forest extent maps
- **Goal:** Retrieve ALOS (Advanced Land Observing Satellite) maps
- **Task:** Download forest extent maps from ALOS
- **Dataset:** ALOS forest extent maps

## 12. Download Glad Forest Map
- **Problem:** Download Global Land Analysis (GLAD) forest maps
- **Goal:** Retrieve GLAD forest extent maps
- **Task:** Download forest maps from GLAD
- **Dataset:** GLAD forest maps

## 13. Download Global Forest Change (Hansen) maps
- **Problem:** Download Hansen Global Forest Change maps
- **Goal:** Retrieve Global Forest Change data
- **Task:** Download and process Hansen maps
- **Dataset:** Hansen forest change maps

## 14. Field boundary segmentation (SAM exploration)
- **Problem:** Segment crop field boundaries
- **Goal:** Segment crop field boundaries using SAM
- **Task:** Use SAM workflow for boundary segmentation
- **Dataset:** FarmVibes.AI data

## 15. Field-level Irrigation Classification
- **Problem:** Estimate irrigation probability
- **Goal:** Generate an irrigation probability map
- **Task:** Use Segment Anything Model (SAM) for classification
- **Dataset:** Segmented crop field data

## 16. Field-level spectral indices
- **Problem:** Compute and visualize spectral indices
- **Goal:** Calculate and display spectral indices
- **Task:** Use Sentinel-2 and SpaceEye data to compute spectral indices
- **Dataset:** Sentinel-2 and SpaceEye imagery

## 17. Green House Gas fluxes
- **Problem:** Calculate GHG emissions and sequestration
- **Goal:** Compute greenhouse gas fluxes for a crop and region
- **Task:** Use environmental data to calculate fluxes
- **Dataset:** Environmental data for specific crops and regions

## 18. Harvest and germination periods
- **Problem:** Infer harvest and germination periods
- **Goal:** Extract crop cycle data from NDVI time-series
- **Task:** Analyze NDVI time series for crop stages
- **Dataset:** NDVI time-series data

## 19. Integration with ADMAg to compute NDVI summary
- **Problem:** Integrate with ADMAg to retrieve NDVI data
- **Goal:** Connect FarmVibes.AI with ADMAg for NDVI computation
- **Task:** Compute NDVI summary using ADMAg integration
- **Dataset:** ADMAg farm data

## 20. Investigating Amazon Rainforest deforestation with SpaceEye
- **Problem:** Analyze Amazon Rainforest deforestation
- **Goal:** Preprocess Sentinel data and analyze deforestation
- **Task:** Use SpaceEye to process Sentinel data and detect deforestation
- **Dataset:** Sentinel imagery over Amazon Rainforest

## 21. Irrigation classification
- **Problem:** Generate irrigation probability map
- **Goal:** Classify irrigation practices using Landsat8 and DEM data
- **Task:** Use remote sensing data to classify irrigation
- **Dataset:** Landsat8 imagery and DEM data

## 22. Land degradation
- **Problem:** Detect land degradation
- **Goal:** Analyze NDVI trends and precipitation data
- **Task:** Detect land degradation using satellite data
- **Dataset:** Landsat images and precipitation data

## 23. Micro climate prediction
- **Problem:** Predict microclimate parameters
- **Goal:** Train model to predict microclimate data
- **Task:** Use weather station and global data to train a microclimate model
- **Dataset:** Global weather data and local weather station data

## 24. Nutrient Heatmap Estimation - Classification
- **Problem:** Estimate soil nutrients heatmap
- **Goal:** Train a model to estimate soil nutrients
- **Task:** Train Random Forest to create nutrient heatmap
- **Dataset:** Soil samples from a farm

## 25. Nutrient Heatmap Estimation - Neighbors
- **Problem:** Estimate soil nutrients based on neighboring samples
- **Goal:** Estimate nutrient heatmap from neighboring soil samples
- **Task:** Use spatial relationships for nutrient estimation
- **Dataset:** Neighboring soil samples

## 26. Nutrient Heatmap Estimation with ADMAg integration
- **Problem:** Estimate soil nutrients heatmap with ADMAg data
- **Goal:** Use ADMAg soil data to estimate a nutrient heatmap
- **Task:** Train Random Forest model using ADMAg data
- **Dataset:** Soil samples retrieved from ADMAg

## 27. Optimal Sensor Placement
- **Problem:** Find optimal sensor placement for soil property collection
- **Goal:** Identify optimal locations for sensor installation
- **Task:** Use satellite imagery to suggest sensor placement locations
- **Dataset:** Satellite imagery

## 28. Optimal Sensor Placement over Segmented Crop Field
- **Problem:** Find optimal sensor locations on segmented crop field
- **Goal:** Estimate sensor placement for segmented fields
- **Task:** Use SAM and satellite imagery to estimate sensor placement
- **Dataset:** Segmented crop field data

## 29. Segment Anything Model Workflow (BingMaps basemap)
- **Problem:** Segment BingMaps basemaps
- **Goal:** Use SAM to segment BingMaps basemaps
- **Task:** Segment BingMaps basemaps with SAM
- **Dataset:** BingMaps basemaps

## 30. Segment Anything Model Workflow (Sentinel-2)
- **Problem:** Segment Sentinel-2 imagery
- **Goal:** Use SAM to segment Sentinel-2 imagery
- **Task:** Segment Sentinel-2 imagery with SAM
- **Dataset:** Sentinel-2 imagery

## 31. Spectral Extension
- **Problem:** Generate high-resolution multispectral data
- **Goal:** Combine drone and Sentinel-2 imagery to create high-res data
- **Task:** Extend spectral data from drone and satellite images
- **Dataset:** High-resolution drone and Sentinel-2 imagery

## 32. Spectral indices
- **Problem:** Compute and visualize spectral indices
- **Goal:** Calculate and visualize spectral indices from Sentinel-2
- **Task:** Compute spectral indices from satellite imagery
- **Dataset:** Sentinel-2 imagery

## 33. Timelapse visualization
- **Problem:** Generate a timelapse of NDVI and SpaceEye data
- **Goal:** Create a timelapse from satellite imagery
- **Task:** Combine NDVI and SpaceEye data for timelapse visualization
- **Dataset:** SpaceEye and NDVI data

## 34. Weed detection
- **Problem:** Detect weed infestations
- **Goal:** Use Gaussian Mixture Model for weed detection
- **Task:** Classify weed-affected regions in raster imagery
- **Dataset:** Raster imagery affected by weeds

## 35. What-if analysis of carbon sequestration
- **Problem:** Analyze potential carbon sequestration scenarios
- **Goal:** Use COMET-Farm API to analyze sequestration
- **Task:** Perform what-if analysis for carbon sequestration
- **Dataset:** Agricultural field data

