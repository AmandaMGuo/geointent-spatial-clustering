# GeoIntent: Graph-based Spatial Clustering for Participatory GIS

**Computational Geospatial Analysis | Spatial Representation | Geographical Uncertainty**

## 1. Project Overview

GeoIntent is a research project exploring how heterogeneous human spatial expressions can be represented, analysed and interpreted computationally.

The original project was conducted as part of the Applying Data Science module (DATA70202) at the University of Manchester, in collaboration with Geodesignhub in 2025.

The industry project aimed to automate the categorisation of citizen-generated spatial geometries and textual responses in participatory planning surveys.

- Institution: University of Manchester
- Industry Partner: Geodesignhub
- Course Leader: Dr Nuno Pinto
- Module Grade: 76/100
- Original Project: February–May 2025

## 2. Research Problem

Different individuals may draw different spatial boundaries when referring to the same geographical location. Variations in position, scale and geometry create challenges for conventional spatial classification.

This project investigates how graph-based spatial relationships can support the computational grouping of heterogeneous geographical expressions.

## 3. My Contribution

Within the collaborative project, I:

- Proposed the methodological logic of the graph-based topological clustering approach.
- Contributed to the Python-based implementation and analysis of spatial relationships.
- Contributed to writing the Geographic Differences chapter, documenting semantic–spatial analysis.
- Contributed to the critical discussion of methodological limitations and potential improvements.

AI-assisted coding was used during implementation. Other components of the collaborative project are attributed to the project team.

## 4. Data and Methodology

The original dataset contained 202 survey responses and 183 spatial records, including 179 valid geometries.

The topological clustering workflow consists of:

1. Survey and spatial data integration.
2. Coordinate reference system transformation.
3. Geometry validity assessment.
4. Geometric feature extraction.
5. Spatial adjacency screening.
6. Pairwise Jaccard similarity calculation.
7. Undirected graph construction.
8. Connected-component extraction.
9. Category-aware spatial grouping.
10. Geometric difference detection.

Core Python libraries include GeoPandas, Pandas, NumPy, Shapely and NetworkX.

## 5. Results

A subsequent reproduction of the original clustering workflow produced:

| Indicator | Result |
|---|---:|
| Valid geometries | 179 |
| Connected graph nodes | 140 |
| Graph edges | 761 |
| Non-isolated connected components | 11 |
| Valid geographical subclasses | 71 |
| Single-object subclasses | 48 |
| Multi-object subclasses | 23 |
| Objects assigned to multi-object subclasses | 131 (73.2%) |

These indicators describe the resulting grouping structure rather than classification accuracy. Independent ground-truth labels were not available for the original analysis.

## 6. Reproducibility and Critical Evaluation

A subsequent AI-assisted code review and reproduction identified several methodological and implementation limitations:

- Dependence on manually specified similarity thresholds.
- Limited tolerance for non-overlapping spatial expressions.
- Transitive chaining in connected-component clustering.
- Potential measurement distortion associated with Web Mercator.
- An index-alignment issue in the geometric difference detection procedure.
- Limited integration of geographical semantics into spatial grouping.

These findings motivate further methodological validation.

## 7. Future Research

Planned research extensions include:

- Parameter sensitivity analysis.
- Controlled experiments on geometric uncertainty.
- Comparison of spatial similarity measures and clustering methods.
- Integration of textual semantics and spatial relationships.
- Geographically grounded spatial reasoning.
- Validation of autonomous geospatial analytical workflows.

The longer-term objective is to investigate how geographical knowledge can support reliable AI-assisted and autonomous GIS.

## 8. Repository Status

The original coursework is completed. Reproducibility checks and methodological extensions are distinguished from the original 2025 project.

## 9. Data Availability

The original survey dataset was provided by the industry partner. Redistribution is subject to the relevant data-sharing permissions.

Synthetic examples will be used for public demonstrations where necessary.

## 10. Acknowledgements

University of Manchester, Geodesignhub, the course teaching team and the collaborative project members.
