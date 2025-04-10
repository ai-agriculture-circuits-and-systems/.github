# Soild Moisture Active Passive
​https://smap.jpl.nasa.gov/

## Data Products
The SMAP baseline science data products are shown in the table below. These data products are made available publicly through two NASA-designated data centers, Alaska Satellite Facility (ASF) and National Snow and Ice Data Center (NSIDC). ASF specializes in SAR data, and NISDC specializes in cryospheric science and land microwave data. You can also browse SMAP data in Worldview.

Level 1 radar data: [ASF DAAC](https://www.asf.alaska.edu/smap/data-imagery/)

Level 1 TB and Level 2-4 products: [NSIDC DAAC](https://nsidc.org/data/smap/smap-data.html)

### Table 1
![image](https://github.com/user-attachments/assets/fee7bd15-d7ef-438c-bd20-60466f635af8)

## Product Information
Level 1B and 1C data products are calibrated and geolocated instrument measurements of surface radar backscatter cross-section and brightness temperatures. L1B_TB_E data product is calibrated brightness temperatures interpolated on EASE-2 grid. Level 2 products are geophysical retrievals of soil moisture on a fixed Earth grid based on Level 1 products and ancillary information; the Level 2 products are output on a half-orbit basis. Level 3 products are daily composites of Level 2 surface soil moisture and freeze/thaw state data. Level 4 products are model-derived value-added data products of surface and root zone soil moisture and carbon net ecosystem exchange that support key SMAP applications and more directly address the driving science questions.

In total, the SMAP mission has generated 24 distributable data products representing four levels of data processing. Level 1 products contain instrument-related data and appear in granules that are based on half orbits of the SMAP satellite. The Northernmost and Southernmost orbit locations demarcate half orbit boundaries. Level 2 products contain output from geophysical retrievals that are based on instrument data and also appear in half orbit granules. Level 3 products are daily global composites of the Level 2 geophysical retrievals for an entire UTC day. Level 4 products contain output from geophysical models utilizing SMAP data.

There are five, L2 soil moisture products resulting from the radar and radiometer data streams. L2_SM_A is a high-resolution research-quality soil moisture product that is mostly based on the radar measurements and is posted at 3 km. L2_SM_P is soil moisture derived from the radiometer brightness temperature measurements and is posted at 36 km. L2_SM_P_E is soil moisture derived from the Backus-Gilbert interpolated radiometer brightness temperature measurements and is posted at 9 km. L2_SM_AP is a combination active and passive (radar and radiometer) product that produces soil moisture estimates at 9 km resolution. L2_SM_SP is a combination Sentinel-1 active and SMAP passive (radar and radiometer) product that produces soil moisture estimates at 3 km resolution.

The radar-only soil moisture (L2_SM_A) is a fine-resolution (3 km) soil moisture estimate derived from high-resolution radar backscatter data (L1C_S0_HiRes). Although the L2_SM_A data product is unlikely to be as accurate as the L2_SM_P and L2_SM_AP products, it produces useful soil moisture information at higher spatial resolution. L2_SM_A produces radar backscatter values aggregated to 3 km during the early stages of its processing. This data set, along with water body and freeze/thaw flags generated from the radar data, is made available during data processing to the other products as input.

The combined radar/radiometer soil moisture product L2_SM_AP is posted on a 9 km Equal Area Scalable Earth-2 (EASE2) grid [1] that is nested consistently with the 36 km and 3 km grids used by other SMAP products. It uses both the high-resolution radar backscatter gridded at 3 km and the radiometer brightness temperature data gridded at 36 km. L2_SM_AP combines the two data streams to produce disaggregated brightness temperatures posted at 9 km. The retrieval algorithm used to estimate soil moisture from the disaggregated 9 km brightness temperatures uses the same approach as the L2_SM_P radiometer-only soil moisture product. The ancillary data inputs and implementation of the L2_SM_AP may differ from those used by L2_SM_P because of the spatial resolution differences at 9 and 36 km.

L3_FT_A, the SMAP freeze/thaw product based on radar data, consists of a daily composite of landscape freeze/thaw state for the boreal land region north of 45N latitude output on a polar EASE2 grid at 3 km. It is derived from high resolution radar data (L1C_S0_HiRes half-orbits) using both the AM (descending) and PM (ascending) overpasses. The L1C_S0_HiRes AM data will also be utilized to generate a freeze/thaw binary state flag for use in the L2/3_SM product algorithms. L3_FT_P and L3_FT_P_E are freeze/thaw products, derived from L1C_TB and L1C_TB_E products, respectively.

L1B_TB_NRT and L2_SM_P_NRT are near time products, corresponding to L1B_TB and L2_SM_P, generated for use by operational users, who need a latency of under 3 hours. They are created using the latest available ancillary data and spacecraft and antenna attitude data to reduce latency. They are not as accurate as the higher quality products, L1B_TB and L2_SM_P, and are not recommended for science users.

SMAP measurements provide direct sensing of soil moisture in the top 5 cm of the soil column. However, several of the key applications targeted by SMAP require knowledge of root zone soil moisture in the top 1 m of the soil column, which is not directly measured by SMAP. As part of its baseline mission, the SMAP project has been producing model-derived value-added Level 4 data products to fill this gap and provide estimates of root zone soil moisture that are informed by and consistent with SMAP surface observations. Such estimates are obtained by merging SMAP observations with estimates from a land surface model in a data assimilation system. The land surface model component of the assimilation system is driven with observations-based meteorological forcing data, including precipitation, which is the most important driver for soil moisture. The model also encapsulates knowledge of key land surface processes, including the vertical transfer of soil moisture between the surface and root zone reservoirs. Finally, the model interpolates and extrapolates SMAP observations in time and in space, producing 3-hourly estimates of soil moisture at a 9 km resolution. The SMAP L4_SM product thus provides a comprehensive and consistent picture of land surface hydrological conditions based on SMAP observations and complementary information from a variety of sources.

The L4_C algorithms utilize daily soil moisture and temperature inputs with ancillary land cover classification and vegetation gross primary productivity (GPP) inputs to compute the net ecosystem exchange (NEE) of carbon dioxide with the atmosphere over global vegetated land areas (with an emphasis on boreal areas north of 45N latitude). Carbon NEE is a fundamental measure of the balance between carbon uptake by vegetation and carbon losses through autotrophic and heterotrophic respiration.

The Table 1 specifies several important characteristics of the SMAP baseline data products. Among these are:
- the product short name – these names provide a short hand method to differentiate among the products
- a very brief product description – additional SMAP project documents provide complete specifications of the format and the content of each data product; the SMAP DAACs have made these documents available to the user community
- product spatial resolution or grid posting – the resolution of some Level 1 products is based on the size of the Instantaneous Field of View (IFOV) of the radar or radiometer instrument, while the resolution of higher-level products is based on the selected grid spacing
- product latency to the user community – latency measures the time between the acquisition of the first element in the data product and the time the product is available for use at one of the SMAP Data Centers. Although the latencies listed in Table 2 are being used by the project to construct the data processing system, the SMAP project will do its best to deliver products sooner, whenever possible

## Science Algorithms
The SMAP science data products will be generated on the Science Data System production system using science algorithm software. The science software is based on algorithms for each product described in the [Algorithm Theoretical Basis Documents (ATBDs)](https://smap.jpl.nasa.gov/documents).

## Data Product Availability and Latency
SMAP data management is governed by NASA's Earth Science Data Policy (adopted in 1991). NASA has developed policy implementation, practices, and nomenclature that Earth science missions use to comply with policy tenets.

[NASA Earth Science Data Policy](http://science.nasa.gov/earth-science/earth-science-data/data-information-policy/)

Product latency to the user community is the measure of time between the observation acquisition of instrument data by the observatory and the time the product is available to the public at the SMAP Data Centers.

The SMAP data latency requirements on delivering data products to the science team and to the community is:
- Level 1 products (within 12 hours of acquisition)
- Level 2 products (within 24 hours of acquisition)
- Level 3 products (within 50 hours of acquisition)
- Level 4 products (within 7 days for soil moisture and 14 days for carbon net ecosystem exchange)

## Data Level Definitions
The SMAP data level definitions follow the standard terminology of the [NASA Earth Observing System Data and Information System (EOSDIS)](http://science.nasa.gov/earth-science/earth-science-data/data-processing-levels-for-eosdis-data-products/).

### Data_product_level_table
![image](https://github.com/user-attachments/assets/ec3ffba8-9b86-4f92-97b1-7ce8279b1d6a)

## Data Maturity Levels

[Description](http://science.nasa.gov/earth-science/earth-science-data/data-maturity-levels/)

The SMAP mission has made science data products available to the public through two NASA-designated Earth science data centers, the Alaska Satellite Facility (for Level 1 radar products) and the National Snow and Ice Data Center (for all other products).

SMAP will coordinate the release of data product versions with the data center and will ensure the completeness and accuracy of quality control information and validation status of the data products. There was a calibration and validation (Cal/Val) phase during the science mission that followed the 90-day post launch in-orbit commissioning (IOC) phase. The duration of the Cal/Val phase was 6 months for Level 1 products and 12 months for Level 2 through Level 4 products.

The initial "beta" release of Level 1 products was made 3 months after IOC. Level 2 to Level 4 beta products were released 6 months after IOC. At the end of the Cal/Val phase the data products were determined to attain the level of "validated".

Following the initial beta releases of data to the data center, subsequent releases will follow the latencies shown in the data products table (above). Latency is defined as the average time under normal operating conditions between data acquisition by the SMAP observatory and delivery of the data to the data center.

Detailed product information from the SMAP Handbook can be found via the links below:
- [Soil Moisture Data Products](https://smap.jpl.nasa.gov/system/internal_resources/details/original/178_SMAP_Handbook_FINAL_1_JULY_2014_Web.pdf#page=57)
- [The Value-Added L4_SM Soil Moisture Product](https://smap.jpl.nasa.gov/system/internal_resources/details/original/178_SMAP_Handbook_FINAL_1_JULY_2014_Web.pdf#page=95)
- [Carbon Cycle Data Products](https://smap.jpl.nasa.gov/system/internal_resources/details/original/178_SMAP_Handbook_FINAL_1_JULY_2014_Web.pdf#page=107)

## Science Data System
The SMAP Science Data System (SDS) processes radar and radiometer instrument data downloaded from the SMAP observatory into [Science Data Products](http://smap-archive.jpl.nasa.gov/science/dataproducts/) provided to the science community for research and applications. The SDS is designed to process and distribute data products in a timely manner as required to meet mission objectives. The SDS facility includes computer hardware dedicated to operational data production as well as hardware for use by the SMAP science algorithm development team to enhance algorithmic accuracy and performance.

![image](https://github.com/user-attachments/assets/44ac2506-5084-459a-b66a-2f9aefa6aada)

SMAP Science Data System architecture and data flows

The key SDS operations functions are:
- Ingest instrument and ancillary data to generate Level 1 through Level 4 science data products.
- Support calibration and validation of science data products
- Provide data access to Project, Science, and Flight Engineering teams
- Regenerate science data products using refined algorithms
- Manage and make available validated products to the SMAP data centers
- Maintain the SDS production and testbed systems

The Science Data System is housed primarily at the Jet Propulsion Laboratory (JPL) in Pasadena, California. JPL is responsible for implementation of software to generate Level 1 radar instrument data products and Level 2 and Level 3 geophysical data products. The Goddard Space Flight Center (GSFC) in Greenbelt, Maryland houses components of the SDS and is responsible for implementation of software to generate Level 4 geophysical data products. The Level 1 radiometer instrument data products are jointly developed by both JPL and GSFC.

The Soil Moisture Active/Passive (SMAP) Science Data System (SDS) provides two environments for the Science Algorithm Development Team (ADT) and the CalVal team. The SDS Testbed, and Offline Algorithm Staging and Input System (OASIS).

The SDS Testbed is a full development environment and serves as a centralized facility to encourage the sharing of tools and data across multiple project elements. The Testbed supports algorithm software development and enhancements, as well as houses Research & Analysis tools that assess current output products and provides insights for algorithm correction and improvements.

The second environment, Offline Algorithm Staging and Input System (OASIS) is a flexible independent instance of the SDS production system to generate large quantities of evaluation products. OASIS is used for moderate-scale reprocessing of data with updated algorithms. All data flows are under the control of the local software and catalog. It includes its own separate and independent life-of-mission storage this is mirrored to the Research & Analysis system for cal/val analysis. OASIS provides a fast turn-around of products from new/enhanced algorithms and can process 45 days of Level 1 radar products in seven (7) days using 30 nodes, and can process five (5) months of Level 2 and Level 3 data in seven (7) processing days using 13 nodes.

[SDS Testbed](http://smap-archive.jpl.nasa.gov/science/SDS/SDSTestbed/)

## Validation Dataset Collection
The Testbed currently hosts over 100 GBytes of data for validation of SMAP mission output. Sources of these data sets include in-situ, airborne, and spaceborne instruments. The testbed hosts a collection of data from the European Soil Moisture Ocean Salinity (SMOS) mission that are used for SMAP algorithm development and validation.

![image](https://github.com/user-attachments/assets/24add02c-34a4-428d-8ca5-737b84378d2a)
Image of composite SMAP data from May 21-May 23, 2015
Retrieved soil moisture based on the SMAP “active” and “passive” radiometer data. SMAP Active-Passive Soil Moisture Product (9 km). Three Days Composite May 21st to May 23rd, 2015.

## Algorithm Development
The SMAP team employs the testbed to implement and evaluate alternative algorithmic approaches. Current versions of these algorithms can ingest multiple versions of data sets as well as data collected from field validation campaigns.

## Data Processing
Multiple ancillary data sets required for processing reside on the testbed. Output data products are converted to the HDF5 standard format that SMAP will use for distributed data products. Model data sets that contain SMAP Data Products in standard HDF5 can be made available to potential users in the software development phase.

![image](https://github.com/user-attachments/assets/a8a191d7-cda1-48d8-8a1c-bcf305b81107)
This design traces physical processes recorded by instruments and modeled by algorithms that convert instrument data into geophysical quantities. SMAP scientists plan to generate components for each of the diagrammed physical processes on the testbed, and employ those components to test retrieval algorithms.

## Distribution Portal
The testbed architecture currently includes a distribution portal. The portal provides access to a subset of the SMAP data products that reside on the testbed. Current access to the portal is limited to members of the SMAP Science Team.

The SDS operational data have been automatically distributed through DAACs for archive and distribution to users.

[National Snow and Ice Data Center SMAP data](https://nsidc.org/data/smap/smap-data.html)

[Alaska Satellite Facility SMAP data](https://asf.alaska.edu/data-sets/sar-data-sets/smap/smap-data-and-imagery/)

