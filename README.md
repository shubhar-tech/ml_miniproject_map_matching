# Map Matching using Machine Learning

## Project Overview

This mini project focuses on **map matching**, which is the process of matching GPS trajectory points to the most likely roads in a road network.

GPS data can contain noise, missing points, and positional errors. Therefore, directly plotting GPS coordinates may not always represent the actual road followed by a vehicle. Map matching helps identify the correct road segments corresponding to the recorded GPS trajectory.

In this project, GPS data, road network data, and a ground-truth route are used to explore and develop a machine learning based map-matching approach.

---

## Objectives

- Explore and preprocess GPS trajectory data.
- Understand the structure of the road network.
- Visualize GPS points and road segments.
- Perform map matching between GPS observations and the road network.
- Compare the predicted route with the ground-truth route.
- Evaluate the performance of the map-matching approach.
- Understand the effect of GPS noise and preprocessing on route prediction.

---

## Dataset / Files

The project contains the following files:

| File | Description |
|------|-------------|
| `01_Data_Exploration_and_Preprocessing (7) (1).ipynb` | Jupyter Notebook containing data exploration, preprocessing, analysis and machine learning implementation. |
| `gps_data.txt` | GPS trajectory data used as input for map matching. |
| `road_network.txt` | Road network information used to identify possible road segments. |
| `ground_truth_route.txt` | Actual/ground-truth route used for comparison and evaluation. |
| `Map_Matching_ML_Mini_Project.pptx` | Project presentation containing the methodology, results and conclusions. |

---

## Methodology

The project follows these major steps:

### 1. Data Exploration

The GPS and road network datasets are loaded and examined to understand:

- Number of records
- Coordinate information
- Data structure
- Missing values
- Possible GPS noise
- Road network structure

### 2. Data Preprocessing

The raw data is cleaned and prepared before applying the map-matching algorithm.

The preprocessing stage may include:

- Handling missing values
- Removing invalid coordinates
- Converting data into suitable numerical formats
- Checking duplicate or inconsistent records
- Preparing GPS points and road network information

### 3. GPS Trajectory Analysis

The GPS coordinates are analysed to understand the movement of the vehicle.

The trajectory is visualized to observe the recorded path and identify possible deviations caused by GPS errors.

### 4. Road Network Analysis

The road network is processed to identify available road segments and their relationships.

The GPS points are then compared with nearby road segments to determine the most likely road followed by the vehicle.

### 5. Machine Learning / Map Matching

Features derived from GPS observations and road segments are used for the map-matching process.

The model/algorithm determines the most suitable road segment for each GPS observation.

### 6. Route Evaluation

The predicted route is compared with the ground-truth route.

The comparison helps determine how accurately the system maps noisy GPS observations to the actual road network.

---

## Technologies Used

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Machine Learning
- GPS / Geospatial Data Processing

---

## Project Structure

```text
Map_Matching_ML_Mini_Project/
│
├── 01_Data_Exploration_and_Preprocessing (7) (1).ipynb
├── gps_data.txt
├── road_network.txt
├── ground_truth_route.txt
├── Map_Matching_ML_Mini_Project.pptx
└── README.md
