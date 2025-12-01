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

* **Source**: [Facebook dataset](https://snap.stanford.edu/data/ego-Facebook.html)

* **Description:**
This dataset contains 10 ego networks (friends list) from Facebook, where each ego network represents a person/entity (called the ego node), its immediate friends (local neighborhood), along with the connections among these friends if any.

For each ego network, there are 5 corresponding files:
* `nodeId.edges`: contains the connections (edges) between friends within the ego network for the ego node identified by 'nodeId'. All nodes listed in this file are direct neighbours (friends) of the ego node.
* `nodeId.circles`: contains the social circles or friend groups (user-defined communities) for the ego node 'nodeId'. Each line in this file represents one social circle, listing the node IDs of friends (nodes) that belong to that social circle.
* `nodeId.feat`: contains the feature data for each friend in the ego network (those appearing in the edges file).
* `nodeId.egofeat`: contains feature data specific to the ego node 'nodeId'.
* `nodeId.featnames`: contains the names/descriptions of the feature dimensions, where features are binary indicators: 1 if the user has the property and 0 otherwise.

**Network Type**: Undirected graph  
**Domain**: Social media (friendship connections)


### Dataset 2: Email Communication Network (Email-Eu-Core)

* **Source**: [Email-Eu-Core dataset](https://snap.stanford.edu/data/email-Eu-core.html)

* **Description:**
This dataset represents email communication within a large European research institution. The network was generated using anonymized email data, capturing all incoming and outgoing emails between members of the institution. An edge (u, v) exists in the network if person u sent person v at least one email. The emails only represent communication between institution members (the core), and the dataset does not contain incoming messages from or outgoing messages to the rest of the world.

The dataset contains the following file:
* `email-Eu-core.txt`: contains the directed edges of the email network. Each line represents an email communication with the format: `source_node target_node`, where source_node sent at least one email to target_node.


**Network Type**: Directed graph  
**Domain**: Email communication network (professional/institutional)
