
---

# Seismic Analysis Based on Machine Learning Algorithms

**Prepared by: Shayan Mansournia**
**Date: March 12, 2025 (Esfand 22, 1403)**

## Introduction

This project focuses on analyzing seismic activities in the Middle East using machine learning (ML) algorithms. The primary dataset, `MiddleEast_EQ.csv`, contains earthquake records with features such as date, time, longitude, latitude, depth, magnitude, and region. The initial phase of the project involves data exploration and visualization to understand the distribution and characteristics of seismic events. This report outlines the methodology, data preprocessing, and visualization techniques used.

---

## Methodology

### 1. Importing Libraries

The project begins by importing essential Python libraries for data manipulation, visualization, and analysis. These libraries provide tools for numerical operations, data management, and plotting.

---

### 2. Loading the Data

The dataset is loaded from a CSV file located at a specified path and stored in a suitable data structure for further processing.

#### Dataset Overview

* **Number of Rows**: 5,000 entries
* **Number of Columns**: 10
* **Column Names and Types**:

  * `Year`: Year of the earthquake (integer).
  * `Month`: Month of the earthquake (integer).
  * `Day`: Day of the earthquake (integer).
  * `Time`: Time of the event (string, e.g., "08:46:23").
  * `Lat`: Latitude of the earthquake epicenter (float).
  * `Lon`: Longitude of the earthquake epicenter (float).
  * `Depth`: Earthquake depth in kilometers (float).
  * `Mag`: Earthquake magnitude (float).
  * `Region`: Geographical region of the event (string).
  * `Timestamp`: Unix timestamp of the event (integer).

The first five rows of data illustrate recent earthquakes in 2025, including events in Iran, Qatar, Afghanistan, and Georgia.

#### Data Summary

Data inspection revealed no missing values— all 5,000 entries are fully populated across all columns.

---

### 3. Data Visualization

To explore the seismic data, four types of visualizations were created:

#### 3.1 Earthquake Magnitude Histogram

* **Purpose**: To analyze the distribution of earthquake magnitudes.
* **Observation**: The majority of earthquakes have moderate magnitudes (e.g., between 4.0 and 5.0 on the Richter scale).

#### 3.2 Scatter Plot: Depth vs. Magnitude

* **Purpose**: To investigate potential correlations between earthquake depth and magnitude.
* **Observation**: Events are mostly concentrated at shallow depths (e.g., around 10 km), with a wide range of magnitudes.

#### 3.3 Scatter Plot: Earthquake Locations (Latitude vs. Longitude)

* **Purpose**: To visualize the geographical distribution of earthquake epicenters.
* **Observation**: Three distinct clusters were identified:

  * **Northwest Cluster**: (Longitude 35–50°, Latitude 35–42.5°), with the highest density.
  * **Northeast Cluster**: (Longitude 55–70°, Latitude 37.5–42.5°), with medium density.
  * **Southern Cluster**: (Longitude 35–70°, Latitude 22.5–32.5°), forming a curved distribution.

#### 3.4 Bar Chart: Top 10 Regions with Most Earthquakes

* **Purpose**: To identify regions with the highest seismic activity.
* **Observation**: The chart highlights the most frequently affected regions, providing insights into seismic hotspots across the Middle East.

---

## Results and Observations

1. **Magnitude Distribution**: Most earthquakes fall within the moderate magnitude range, indicating regular seismic activity in the region.
2. **Depth and Magnitude**: No clear correlation between depth and magnitude was observed, but a concentration of shallow events was noted.
3. **Geographical Distribution**: Three main clusters were identified, representing seismic activity zones in the Middle East:

   * Northwest (high density),
   * Northeast (medium density),
   * South (curved distribution).
4. **Frequent Regions**: Areas with the highest number of earthquakes were highlighted, useful for further analysis.

---

## Next Steps

* **Data Preprocessing**: Convert the time column into a usable format and standardize the dataset.
* **ML Modeling**: Apply clustering algorithms to confirm observed clusters and attempt earthquake prediction.
* **Advanced Analysis**: Examine correlations and temporal patterns to enhance the understanding of seismic behavior.

---

## Conclusion

This preliminary report shows that seismic data from the Middle East presents identifiable geographical and statistical patterns that can serve as a foundation for more advanced analysis using machine learning. The visualizations provide an initial understanding of earthquake distributions and set the stage for the next phases of the project.

---

**End of Report**

---
