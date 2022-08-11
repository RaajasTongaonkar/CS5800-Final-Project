# CS5800-Final-Project
Repo for the final project of Summer '22 CS5800 class


This GitHub repo contains all the code we used for our CS5800 (Summer '22) final project - Blue Bikes in Boston

## Running Submap generation
### File to run - CS5800_final_proj_submap_generation.ipynb
### File to upload - Blue_Bike_Stations.csv
This creates the submap and graph from the dataset. Upload the Blue_Bike_Stations.csv file before running. 

First it preprocesses the data and then creates edges between all remaining nodes. Then, the edges above the threshold value are dropped. The remaining edges and nodes then form the adjacency matrix. Two user-defined classes are created and used for ease of functioning later, Graph and Node.

## Running Prim's algorithm
### File to run - MST_Prim.py
### File to upload - Graph g.pkl

This script runs Prim's algorithm to create the MST on the given Graph g which would be loaded in Graph and Node classes.
The graph that would be plotted contains labels of the station names and distances between two stations.
It also prints the total distance of the MST that connects all of the Boston Bluebikes stations.


## Running Djikstra's algorithm
### File to run - CS5800_final_project_djikstra's_implementation.ipynb
### Files to upload - Dataframe.pkl, Graph g.pkl

Run the cell where the two classes Graph and Node are defined before running the code to load the dataframe and the graph.
This script runs the Djikstra's algorithm on the given Graph and gives the shortest path between the source and destination. 
You can give a part of the station name and choose one of the stations which has that substring in its name. 
Changing group size gives an alternative path based on the number of docking stations at the intermediary stations, returning an error if such a route is not possible.


## Outputs
<img width="790" alt="mst_no_labels" src="https://user-images.githubusercontent.com/31932749/184040974-e5bc6c3b-1021-4b1a-980e-37a10181f2a2.png">
Minimum Spanning Tree on the graph, with no labels


![mst_with_labels](https://user-images.githubusercontent.com/31932749/184041026-e3b04974-b24a-46ac-9eca-e41a2f538ebb.png)
Minimum Spanning Tree on the graph, with label


![Djikstra's path](https://user-images.githubusercontent.com/31932749/184041047-2e1e7c61-87f3-464b-8915-9c1f26436140.png)
Shortest path from Djikstra's algorithm


![Djikstra's path larger group size](https://user-images.githubusercontent.com/31932749/184041075-65d3e41f-69c6-4d1f-ac03-12974d030377.png)
Shortest path from Djikstra's algorithm with a larger group


