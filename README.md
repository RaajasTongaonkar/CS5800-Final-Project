# CS5800-Final-Project
Repo for the final project of Summer '22 CS5800 class


This GitHub repo contains all the code we used for our CS5800 (Summer '22) final project - Blue Bikes in Boston

## Running Submap generation
### File to run - CS5800_final_proj_submap_generation.ipynb
### File to upload - Blue_Bike_Stations.csv
This creates the submap and graph from the dataset. Upload the Blue_Bike_Stations.csv file before running. 

First it preprocesses the data and then creates edges between all remaining nodes. Then, the edges above the threshold value are dropped. The remaining edges and nodes then form the adjacency matrix. Two user-defined classes are created and used for ease of functioning later, Graph and Node.

## Running Prim's algorithm
### File to run - 
### File to upload



## Running Djikstra's algorithm
### File to run - CS5800_final_project_djikstra's_implementation.ipynb
### Files to upload - Dataframe.pkl, Graph.pkl

Run the cell where the two classes Graph and Node are defined before running the code to load the dataframe and the graph.
This script runs the Djikstra's algorithm on the given Graph and gives the shortest path between the source and destination. 
You can give a part of the station name and choose one of the stations which has that substring in its name. 
Changing group size gives an alternative path based on the number of docking stations at the intermediary stations, returning an error if such a route is not possible.
