# Vegetation Assessment using Google Earth Engine (GEE) - NDVI, MNDWI, and VFC

This repository contains scripts and data related to **vegetation assessment** based on the calculation of **NDVI** (Normalized Difference Vegetation Index), **MNDWI** (Modified Normalized Difference Water Index), and **VFC** (Vegetation Fraction Cover) derived from **MODIS** and **Landsat** datasets. The analysis was processed using **Google Earth Engine (GEE)** and is intended to assist in environmental monitoring and land cover change studies.

## Dataset Information:
- **MODIS Data**: MODIS (Moderate Resolution Imaging Spectroradiometer) provides global data at moderate spatial resolution, useful for monitoring large-scale vegetation patterns.
- **Landsat Data**: Landsat satellite imagery provides higher spatial resolution, ideal for more detailed vegetation analysis.
- **GEE (Google Earth Engine)**: The data processing was carried out using **Google Earth Engine**, which provides cloud-based tools for large-scale geospatial data analysis.

## Vegetation Indices Calculated:
### 1. **NDVI (Normalized Difference Vegetation Index)**
   NDVI is a measure of vegetation health. It is computed from the **red** and **near-infrared** bands and helps identify areas of healthy vegetation.

   Formula: 
   \[
   \text{NDVI} = \frac{(\text{NIR} - \text{RED})}{(\text{NIR} + \text{RED})}
   \]
   
### 2. **MNDWI (Modified Normalized Difference Water Index)**
   MNDWI is used to monitor water bodies, and it is sensitive to changes in surface water content.

   Formula:
   \[
   \text{MNDWI} = \frac{(\text{Green} - \text{SWIR})}{(\text{Green} + \text{SWIR})}
   \]
   
### 3. **VFC (Vegetation Fraction Cover)**
   VFC indicates the fraction of land covered by vegetation. This index helps assess land cover and changes in vegetation extent.

   Formula: Typically derived from **NDVI** thresholds that classify pixels into different vegetation classes.

## Data Processing:
The data was processed using the following steps:
1. **Data Acquisition**: MODIS and Landsat datasets were retrieved from their respective sources.
2. **Data Preprocessing**: Cloud masking and atmospheric correction were applied to both MODIS and Landsat images.
3. **Calculation of NDVI, MNDWI, and VFC**: Vegetation indices were calculated using **Google Earth Engine** with MODIS and Landsat reflectance data.
4. **Analysis and Visualization**: The processed data was analyzed and visualized in **Google Earth Engine**, with outputs provided as **GeoTIFF** files for further analysis in **ArcGIS** or **QGIS**.

## Geographical Coverage:
- **Latitude**: [Your study area latitude range]
- **Longitude**: [Your study area longitude range]

## License:
This repository is made available under the **CC BY 4.0** (Creative Commons Attribution 4.0 International License), allowing reuse with proper attribution. You are free to use, modify, and distribute the data, provided you credit the source.

Alternatively, if you prefer to make the data freely available for reuse without any restrictions, you can use **CC0** (Public Domain Dedication).

## How to Use:
1. **Download the Data**: The GeoTIFF files are available for download in this repository.
2. **Run the Scripts**:
   - The provided **Google Earth Engine (GEE) scripts** calculate **NDVI**, **MNDWI**, and **VFC**.
   - You can open and run the scripts in the **Google Earth Engine** platform (https://code.earthengine.google.com/).
3. **Visualize the Results**:
   - The **GeoTIFF** outputs can be loaded into **ArcGIS** or **QGIS** for further analysis and visualization.

## Citation:
If you use this code or the data in your research, please cite the following:
Nawaz, T., [2025]. Vegetation Assessment Using NDVI, MNDWI, and VFC from MODIS and Landsat. Retrieved from (https://github.com/Tauqeernawaz). 

## References:
- **MODIS Data**: [MODIS Data Portal](https://modis.gsfc.nasa.gov/data/)
- **Landsat Data**: [Landsat Data Portal](https://landsat.visibleearth.nasa.gov/)
- **Google Earth Engine**: [Google Earth Engine Documentation](https://developers.google.com/earth-engine)

