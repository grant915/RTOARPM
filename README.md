# RTOARPM
This repository contains the instances and results used in the paper "Robust Drone Selective Routing in Humanitarian Transportation Network Assessment".

This paper focuses on a variant of the team orienteering arc routing problem (TOARP) where the network is a multigraph. In particular, the proposed problem exhibits several unique characteristics: (i) there exists more than one edge between two nodes for which the corresponding benefits from the exploration are different; (ii) the targets are associated with undirected edges; and (iii) Uncertainty in service time is considered. Those characteristics not only makes the conventional modeling approach invalid, but also enlarges the solution space and deteriorates the computational efforts. Considering novel features, we refer the proposed problem as robust team orienteering arc routing problem on a multigraph (RTOARPM).

# Instances
This instances set includes 15 RTOARPM instances, and each instance (named RTOARPM_m_n) is composed of a node file (named nodes_m_n_1.txt) and an arc file (named arcs_m_n_1.txt). 

In the node file, the first line reports the number of available vehicles.
