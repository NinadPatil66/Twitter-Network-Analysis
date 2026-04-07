# Twitter-Network-Analysis
Analyzing Twitter follower data using Python & NetworkX (Graph Analysis)

## Goal - 
Spot key influencers, find out who follows who, and discover mutual connections between users.

## NetworkX - 
NetworkX - NetworkX is a powerful Python library used for the creation, manipulation, and study of the structure, dynamics, and functions of complex networks. It is the industry standard for network analysis in Python. If you are trying to analyze a massive graph with billions of nodes (like the entire global web), you might find it a bit slow. In those rare "Big Data" cases, people often move to tools like graph-tool or igraph, which are built on C++.

It supports many types of graphs, including:
- Undirected Graphs: Connections go both ways (like a Facebook friendship).
- Directed Graphs (DiGraphs): Connections have a direction (like a Twitter/X "follow").
- Multigraphs: Where multiple edges can exist between the same two nodes.

Instead of writing complex math from scratch, NetworkX comes with a massive library of ready-to-use algorithms:
- Shortest Path: Finding the quickest route between two points (Dijkstra’s algorithm).
- Centrality: Identifying the "most important" or "most influential" nodes in a network.
- Clustering: Detecting communities or groups within a larger crowd.

- You can easily convert data from Pandas DataFrames or NumPy arrays into a NetworkX graph, analyze it, and then export the results.
- You can attach "attributes" to nodes and edges. For example, a node representing a city can store its population, and an edge representing a road can store its length or speed limit.

# Tech Stack - 
1) Python
2) NetworkX
