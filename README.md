# COMP5313 Large Scale Networks
This unit focuses on the analysis of large-scale complex networks using graph theory and network science. 
Key topics include small-world properties, community detection, triadic closures, centrality measures, and signed/directed networks. Students develop skills in modeling, analysing, and visualising real-world network structures.

## Project: Structural Balance of Harry Potter’s Character Network
### Summary
* Type: Individual project
* Objective: Analyse the structural balance of a signed, directed character network from the Harry Potter universe using triadic decomposition, and evaluate how directionality affects balance.

### Problem
How balanced is the Harry Potter character network, and does considering the direction of relationships alter its balance score?

### Solution
* Built a signed, directed network of 65 characters and 456 interactions using data from data.world (original URL I referenced but it doesn't work anymore: https://data.world/harishkgarg/harry-potter-universe).
* Conducted two experiments:
    1. With direction & sign
        * Applied triadic analysis using the method proposed by Dinh et al. (2020) to compute structural balance based on semi-cycles.
    1. Without direction
        * Transformed the network into an undirected graph and analysed triangle-based balance.
* Results showed:
    * 93.11% balance when considering direction and sign.
    * 82.84% balance without direction, indicating directionality plays a crucial role in accurately modeling relational balance.

Network visualisation in Gephi was used to show clusters and edge polarity (positive/negative).

### Tools & Technologies
* Languages & Libraries: Python, NetworkX, NumPy, Pandas, Matplotlib
* Visualisation: Gephi, NetworkX
* Techniques:
    * Structural balance analysis using triads and semi-cycles
    * Network flattening (Diesner & Evans method)
    * Clustering coefficient, density, and triadic census
    * Community detection (Louvain method)
