# RTOARPM
This repository contains the instances and results used in the paper "Robust Drone Selective Routing in Humanitarian Transportation Network Assessment".

This paper focuses on a variant of the team orienteering arc routing problem (TOARP) where the network is a multigraph. In particular, the proposed problem exhibits several unique characteristics: (i) there exists more than one edge between two nodes for which the corresponding benefits from the exploration are different; (ii) the targets are associated with undirected edges; and (iii) Uncertainty in service time is considered. Those characteristics not only makes the conventional modeling approach invalid, but also enlarges the solution space and deteriorates the computational efforts. Considering novel features, we refer the proposed problem as robust team orienteering arc routing problem on a multigraph (RTOARPM).

# Instances
This instances set includes 15 RTOARPM instances, and each instance (named RTOARPM_m_n) is composed of a node text (named Nodes_m_n.txt) and an arc text (named Arcs_m_n.txt). 

In the node text, the first line reports the number of available vehicles. Lines 2 to the last report the attribute of nodes, including
NodeID;
Type: customer/depot;
Xloc/Yloc: the location on x/y axis.
For example:
Number of drone:  3
NodeID   Type   Xloc   Yloc  
1   customer   0.0   13.76  
2   customer   0.0   24.76  
3   customer   0.0   33.04  
...

The arc text reports the attribute of arcs, including
Nodei/Nodej: the start/end node of the arc;
EucDist: the Euclidean distance of the arc;
IfRoad: equal 1 if there is a road between Nodei and Nodej, 0 otherwise;
RoadLen: the length of the road if there is a road;
RoadScore: the score associated with the road.
For example:
Nodei   Nodej   EucDist   IfRoad   RoadLen   RoadScore  
1   1   0.0   0   -   -  
1   2   11.13   0   -   -  
1   3   19.31   0   -   -  
1   4   12.31   0   -   -  
1   5   5.74   0   -   -  
1   6   5.25   1   5.56   379.0  
...

