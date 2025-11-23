README.md

# Authors:
1. Alexandra Perruchot-Triboulet Rodríguez
2. Lucia Victoria Fernandez Sanchez

# Objective

For this project, we have chosen 2 different graph datasets. For each of them we have:
1. Computed some preliminary statistics and performed analysis on the dataset using some centrality measures and relevant visualisations, including what each graph represents.
2. Compute/detect the communities on the dataset using at least 2 different detection community algorithms and different metrics to evaluate the quality of the communities.

# Datasets

The two data that we have chosen are:
### Dataset 1: Social circles: Facebook

* *Source*: [Facebook dataset](https://snap.stanford.edu/)

* *Description:*
This dataset contains 10 ego networks (friends list) from Facebook, where each ego network represents a person/entity (called the ego node), its immediate friends (local neighborhood), along with the connections among these friends if any.
For each ego network, there are 5 corresponding files:
    * `nodeId.edges`: contains the connections (edges) between friends within the ego network for the ego node identified by 'nodeId'. All nodes listed in this file are direct neighbours (friends) of the ego node.
    * `nodeId.circles`: contains the social circles or friend groups (user-defined communities) for the ego node 'nodeId'. Each line in this file represents one social circle, listing the node IDs of friends (nodes) that belong to that social circle.
    * `nodeId.feat`: contains the feature data for each friend in the ego network (those appearing in the edges file).
    * `nodeId.egofeat`: contains feature data specific to the ego node 'nodeId'.
    * `nodeId.featnames`: contains the names/descriptions of the feature dimensions, where features are binary indicators: 1 if the user has the property and 0 otherwise.


### Dataset 2: ADD NAME OF DATASET 2

* *Source*: [Protein-Protein Interaction (PPI) dataset](https://string-db.org/cgi/download)

* *Description:* This file contains a Protein-Protein Interaction (PPI) network for the organism Homo sapiens (human), sourced from the STRING database (version 12.0). The network represents functional associations between proteins, integrating evidence from various sources

The dataset has been pre-processed with the following filters to reduce file size and focus on higher-confidence interactions:

* Limited to Homo sapiens
* Only includes interactions with a combined confidence score ≥ 400 (on a scale of 0-1000). This filter retains more reliable interactions while excluding speculative ones.
* Duplicate interaction pairs (e.g., A-B and B-A) are removed. Only one entry per interacting pair is included (onlyAB), reducing file size by 50%.


TBD.


