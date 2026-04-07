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

Knowledge Graphs - A Knowledge Graph is a way of organizing and connecting data so that a computer understands not just the words, but the concepts and the relationships between them.

## Main Functions - 
T = nx.from_pandas_edgelist(df, 'FOLLOWER', 'FOLLOWEE', create_using=nx.DiGraph()) - Used to create a NetworkX object (Directed Graph)
T.neighbors(user1) - Since this is a directed graph, this function will return the list of all users which user1 follows (edges directing out)
T.nodes() - Gives a list of all the nodes in the NetworkX object. (Only unique records from the original dataset are present) 
nx.degree_centrality(T) - It gives the total number of edges directing (in or out) from each node in the NetworkX object. It is a list of tuple pairs (node, degree centrality) 

# Tech Stack - 
1) Python
2) NetworkX
