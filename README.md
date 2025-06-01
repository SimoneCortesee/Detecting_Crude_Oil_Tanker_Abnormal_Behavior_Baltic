# Detecting Abnormal Crude Oil Tanker Behavior in the Baltic Sea

This project analyzes AIS (Automatic Identification System) data to detect abnormal behavior of crude oil tankers operating in the Baltic Sea from 2021 to 2025. It also classifies tankers into risk categories using clustering techniques.

## Features

- Detects anomalies such as:
  - Abrupt changes in course
  - "Going dark" behavior (signal loss)
  - Abnormal speed patterns
- Clusters vessels into risk categories based on behavior patterns and static parameters 

## Dataset Requirements

The AIS dataset should include the following columns:

- `DATE TIME (UTC)`
- `MMSI`
- `LATITUDE`
- `LONGITUDE`
- `SPEED`
- `COURSE`
- `NAVSTAT`
- `IMO`
- `NAME`
- `BUILT`
- `FLAGNAME`

## Usage

### 1. Set Up

- Python (latest version recommended)

### 2. Run the Analysis

Follow the notebook sequence below:

1. **`dataframe_construction.ipynb`**
   - Constructs the initial `traffic_df` DataFrame from raw AIS data.

2. **Anomaly Detection**
   - `change_of_course_anomaly_detection.ipynb`
   - `going_dark_anomaly_detection.ipynb`
   - `SPEED_anomaly_detection.ipynb`

3. **Clustering Preparation**
   - `preparing_data_for_clustering.ipynb`: Prepares data for clustering.

4. **Clustering**
   - `Clustering_script.ipynb`: Applies clustering models to categorize vessels by risk.


## License

This project is open source. 

## Author

Created by Simone Cortese — (https://github.com/SimoneCortesee)
