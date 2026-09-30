# Explainable Graph Learning for Prospective Road-Segment Collision Susceptibility and Network Consequence Analysis

## Master's Thesis

This repository contains the implementation for my Master's thesis on prospective road-segment collision susceptibility prediction in Greater London.

## Research Objective

The research investigates whether graph-based machine-learning models can improve prospective road-segment collision susceptibility prediction compared with conventional machine-learning approaches while maintaining interpretable and leakage-safe evaluation.

The primary prediction target is whether a road segment experiences at least one police-reported personal-injury collision in a future period t+1, using only information available through time t.

## Study Area

Greater London, United Kingdom

## Core Data Sources

The project combines:

- OpenStreetMap road-network data
- STATS19 road safety data
- Department for Transport traffic count / AADF data

## Methodology

The planned research workflow is:

1. Construct the Greater London road network.
2. Define and audit road-segment analysis units.
3. Map-match STATS19 collisions to road segments.
4. Match DfT traffic observations to road segments.
5. Construct a road-segment-year dataset.
6. Create leakage-safe historical predictors and future labels.
7. Train conventional machine-learning baselines.
8. Construct a road-segment line graph.
9. Train graph neural network models.
10. Compare, calibrate and explain model predictions.
11. Assess network consequence.
12. Develop a transparent prioritisation framework.

## Models

### Conventional Machine Learning

- Logistic Regression
- Random Forest
- XGBoost
- LightGBM

### Graph Neural Networks

- Graph Convolutional Network (GCN)
- GraphSAGE
- Graph Attention Network (GAT)

GraphSAGE is the primary graph model candidate, but the study does not assume that graph models will outperform conventional models.

## Current Implementation

The first implementation stage focuses on road-network acquisition and inspection.

The current notebook:

`notebooks/01_osm_london_network.ipynb`

performs the following steps:

- installs and imports OSMnx and geospatial libraries
- tests road-network extraction using Westminster
- obtains the Greater London drivable road network
- converts the graph to node and edge GeoDataFrames
- visualizes the road network
- stores the network as GraphML
- exports geographic nodes and edges as GeoPackage files

The network edges provide the initial basis for defining road-segment analysis units. Further segmentation auditing will be performed before constructing the modelling dataset.

## Current Project Status

Completed:

- [x] Google Colab development environment
- [x] OSMnx installation
- [x] Westminster network prototype
- [x] Greater London drivable road-network extraction
- [x] Network visualization
- [x] Node and edge GeoDataFrame conversion
- [x] GraphML network storage
- [x] GeoPackage node/edge storage

Next stages:

- [ ] Road-segment audit
- [ ] STATS19 data inspection
- [ ] Collision map matching
- [ ] DfT AADF integration
- [ ] Road-segment-year panel construction
- [ ] Leakage-safe feature engineering
- [ ] Traditional machine-learning baselines
- [ ] Line-graph construction
- [ ] GNN implementation
- [ ] Explainability analysis
- [ ] Network consequence analysis

## Reproducibility

Raw datasets are kept separate from the source code and are not committed directly to the repository.

The project follows the structure:

data/raw -> data/interim -> data/processed

where original source data are preserved without manual modification.
