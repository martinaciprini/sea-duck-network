# A Complex Network Analysis of Migratory Patterns in Five North American Sea Duck Species

This repository contains the code for the project  
*“A Complex Network Analysis of Migratory Patterns in Five North American Sea Duck Species”*.

The project applies graph-theoretical tools to study migratory connectivity across the full annual cycle of five sea duck species in North America, following and extending the methodological framework of Lamb et al. (2019).

The purpose of this README is to briefly describe the structure of the repository and how the code is organized.

---

## Project Overview

Using processed telemetry-derived habitat centroids provided by Lamb et al., we reconstructed a multi-species, spatially explicit movement network in which:

- *Nodes* represent clustered habitat areas,
- *Edges* represent directed movements between habitats,
- *Weights* account for species-specific sampling effort.

The resulting network was analysed using:
- Centrality measures (betweenness, indegree, outdegree),
- Probability of Connectivity (PC) and its variation (dPC),
- Community structure via the Girvan–Newman modularity algorithm,
- Species-specific and sex-specific subnetworks.

Unlike the original study, we reconstructed the spatial clustering step and adopted a 28-node configuration, requiring a controlled remapping of the original 31-node dataset.

---

## Repository Structure

This repository includes:

- *Data: data provided by Lamb et al.*:  
  [original_data](https://github.com/martinaciprini/sea-duck-network/tree/997ef7436e0fbb7e71dae3708f32e1b0bed4d327/original_data)
- *Data after clustering solution*:  
  [centroids_k28_definitivo.csv](https://github.com/martinaciprini/sea-duck-network/blob/0a4343696161a3729ce50ea1257a983644e839b7/centroids_k28_definitivo.csv)  
  Modified version of the original dataset based on our clustering solution;
- *Global analysis*:  
  [global_analysis](https://github.com/martinaciprini/sea-duck-network/tree/0a4343696161a3729ce50ea1257a983644e839b7/global_analysis)  
  Code for the analysis of the global network;
- *Species-specific analysis*:  
  [species_specific_analysis](https://github.com/martinaciprini/sea-duck-network/tree/0a4343696161a3729ce50ea1257a983644e839b7/species_specific_analysis)  
  Code for species-specific network analyses;
- *Graphs*:  
  [graphs](https://github.com/martinaciprini/sea-duck-network/tree/997ef7436e0fbb7e71dae3708f32e1b0bed4d327/graphs)  
  Figures used in the final report.
  
---

## Global Analysis

This section contains code for analysing the global network, including:

- [Clustering solution](https://github.com/martinaciprini/sea-duck-network/blob/0a4343696161a3729ce50ea1257a983644e839b7/global_analysis/clustering.ipynb):  
  plotting geographical centroids and implementing the clustering algorithm;
- [Nodes and graph plots](https://github.com/martinaciprini/sea-duck-network/blob/0a4343696161a3729ce50ea1257a983644e839b7/global_analysis/graphs_nodes_links_weitghed.ipynb):  
  visualization of the weighted network;
- [Centrality analysis](https://github.com/martinaciprini/sea-duck-network/blob/0a4343696161a3729ce50ea1257a983644e839b7/global_analysis/centrality.ipynb):  
  computation of centrality measures;
- [dPC and modularity](https://github.com/martinaciprini/sea-duck-network/blob/0a4343696161a3729ce50ea1257a983644e839b7/global_analysis/dpc_modularity.ipynb):  
  analysis of connectivity and community structure;

---

## Species-Specific Analysis

This section includes code for analysing species-specific networks:

- [Weighted species-specific networks](https://github.com/martinaciprini/sea-duck-network/tree/0a4343696161a3729ce50ea1257a983644e839b7/species_specific_analysis/weighted_networks):  
  construction of weighted networks for individual species;
- [Centrality measures](https://github.com/martinaciprini/sea-duck-network/tree/0a4343696161a3729ce50ea1257a983644e839b7/species_specific_analysis/centrality):  
  centrality analysis for species-specific networks;
- [dPC analysis](https://github.com/martinaciprini/sea-duck-network/tree/0a4343696161a3729ce50ea1257a983644e839b7/species_specific_analysis/dpc):  
  computation of dPC values for species-specific networks.
