\# Hyderabad Urban Growth and Land-Use Change Analysis



\## Project Overview



This project analyzes urban growth and land-use change in Hyderabad, Telangana, using satellite imagery and machine learning techniques.



Satellite images from \*\*2018 and 2025\*\* are analyzed to identify built-up areas, vegetation, and other land-cover areas. Spectral indices such as \*\*NDVI\*\* and \*\*NDBI\*\* are calculated, followed by Random Forest classification and urban growth analysis.



The project estimates the change in Hyderabad's built-up area between 2018 and 2025.



\---



\## Objectives



\* Analyze satellite imagery of Hyderabad.

\* Calculate NDVI and NDBI.

\* Identify built-up areas.

\* Apply Random Forest machine learning classification.

\* Compare built-up areas between 2018 and 2025.

\* Calculate urban growth percentage.

\* Generate maps and graphs for visualization.



\---



\## Data Source



The satellite imagery used in this project is from \*\*Landsat 8 Collection 2 Level-2 Surface Reflectance\*\* data.



The analysis uses imagery from:



\* \*\*2018\*\*

\* \*\*2025\*\*



The satellite data contains spectral bands required for calculating vegetation and built-up indices.



The raw satellite files are not included in this GitHub repository because of their large file size.



\---



\## Methodology



The project follows these major steps:



1\. Satellite data collection

2\. Image preprocessing

3\. Hyderabad boundary extraction

4\. NDVI calculation

5\. NDBI calculation

6\. Built-up area identification

7\. Random Forest classification

8\. Built-up area calculation

9\. Urban growth calculation

10\. Map and graph generation



\---



\## Spectral Indices



\### NDVI



Normalized Difference Vegetation Index (NDVI) is used to identify vegetation.



Formula:



\*\*NDVI = (NIR - Red) / (NIR + Red)\*\*



Higher NDVI values generally indicate healthier vegetation.



\---



\### NDBI



Normalized Difference Built-up Index (NDBI) is used to identify built-up areas.



Formula:



\*\*NDBI = (SWIR - NIR) / (SWIR + NIR)\*\*



Higher NDBI values generally indicate built-up surfaces.



\---



\## Machine Learning



A \*\*Random Forest Classifier\*\* was used for land-cover classification.



The model used the following features:



\* Red

\* NIR

\* SWIR

\* NDVI

\* NDBI



The classification categories were:



\* Other

\* Vegetation

\* Built-up



The model evaluation showed \*\*100% agreement with the generated pseudo-labels\*\* on the sampled dataset.



This should not be interpreted as 100% real-world classification accuracy because the training labels were generated using threshold-based pseudo-labels rather than independently verified ground-truth data.



\---



\## Hyderabad Urban Growth Results



| Metric                |     Value |

| --------------------- | --------: |

| 2018 Built-up Area    | 71.69 km² |

| 2025 Built-up Area    | 80.35 km² |

| Net Built-up Increase |  8.66 km² |

| Urban Growth          |    12.08% |



The estimated built-up area increased from approximately \*\*71.69 km² in 2018\*\* to \*\*80.35 km² in 2025\*\*.



This represents a \*\*net increase of approximately 8.66 km²\*\*, corresponding to approximately \*\*12.08% urban growth\*\*.



\---



\## Maps



The project generates the following maps:



\* Hyderabad Built-up Area — 2018

\* Hyderabad Built-up Area — 2025

\* Hyderabad NDVI Change

\* Hyderabad NDBI Change

\* Hyderabad Urban Growth Map — 2018 to 2025



\---



\## Graphs



The following graphs are generated:



\* Built-up Area Comparison

\* Urban Growth Percentage

\* Random Forest Feature Importance

\* NDBI vs Machine Learning Built-up Comparison



\---



\## Project Structure



```text

Hyderabad\_Urban\_Growth/

│

├── data/

│   ├── 2018/

│   └── 2025/

│

├── notebooks/

│   └── urban\_growth\_analysis.ipynb

│

├── outputs/

│   ├── maps/

│   ├── graphs/

│   └── results/

│

├── README.md

├── .gitignore

└── requirements.txt

```



The `data/` folder contains the original satellite imagery locally but is excluded from GitHub because of its large size.



\---



\## Technologies Used



\* Python

\* Jupyter Notebook

\* NumPy

\* Pandas

\* Matplotlib

\* GeoPandas

\* Rasterio

\* Shapely

\* Scikit-learn

\* Requests



\---



\## Key Insights



\* Hyderabad's estimated built-up area increased between 2018 and 2025.

\* The estimated net built-up increase was approximately \*\*8.66 km²\*\*.

\* The corresponding urban growth was approximately \*\*12.08%\*\*.

\* NDBI was useful for identifying built-up surfaces.

\* NDVI helped identify vegetation.

\* Random Forest was used to classify land-cover categories.



\---



\## Limitations



\* The analysis uses satellite imagery from selected dates rather than a continuous time series.

\* The Random Forest model was evaluated against pseudo-labels rather than independently verified ground truth.

\* Cloud and seasonal conditions can influence satellite-based indices.

\* Built-up area estimates depend on the selected thresholds and classification approach.

\* The study focuses on Hyderabad district boundaries.



\---



\## Future Improvements



Future versions of the project could include:



\* Multi-year satellite image analysis.

\* More accurate ground-truth land-cover samples.

\* Deep learning-based image classification.

\* Higher-resolution satellite imagery.

\* Automated satellite data downloading.

\* Interactive maps using Folium or Google Earth Engine.

\* Detailed analysis of vegetation and water-body changes.

\* Prediction of future urban expansion.



\---



\## Conclusion



This project demonstrates how satellite remote sensing, spectral indices, geospatial analysis, and machine learning can be combined to study urban expansion.



The analysis indicates that Hyderabad's estimated built-up area increased from \*\*71.69 km² in 2018\*\* to \*\*80.35 km² in 2025\*\*, representing a \*\*net increase of 8.66 km²\*\* and approximately \*\*12.08% growth\*\*.



The project provides a practical example of using Python and machine learning for geospatial and urban-growth analysis.



\---



\## Project Information



\*\*Project Title:\*\* Hyderabad Urban Growth and Land-Use Change Analysis



\*\*Study Area:\*\* Hyderabad, Telangana, India



\*\*Study Period:\*\* 2018–2025



\*\*Domain:\*\* Data Science, Remote Sensing, GIS and Machine Learning



