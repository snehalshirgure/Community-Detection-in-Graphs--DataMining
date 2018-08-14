# Community Detection in Graphs--DataMining

# Project Overview

Implement the Girvan-Newman algorithm using the Spark Framework in order to detect communities in the graph. You
will use ratings.csv dataset (from MovieLens dataset online) in order to find users who have the similar product taste. The goal is to use the Girvan-Newman algorithm to detect communities in an effcient way by programming it within a distributed environment.

# Construct Graph
Each node represents a user. Each edge is generated in following way: In input file, count the number of times that two users rated the same movie. If the number of times is greater or equivalent to 9 times, there is an edge between two users.

# Task 1: Betweenness
You are required to implement Girvan-Newman Algorithm to find betweenness of each edge in the graph. The betweenness function should be calculated only once from the original graph.

# Task2: Detect Community 
You are required to implement betweenness and modularity in this task. You also need to divide the graph into suitable communities, which reaches the highest modularity. When you use the following formula to calculate modularity of partition S of G, you should be aware that Aij and ki kj should change while you delete edges in the graph. You only need to calculate the modularity when a new Community appear. (When you remove edges in the graph, if no Community be divided, you don't need to calculate the modularity). The modularity of the graph will first increase and then decrease, when you found that the modularity decreasing, the highest value before is the highest modularity point.

# Bonus
There are some libraries containing the community detection function.
You can detect communities by using community detection function in
SparklingGraph. The graph is constructed in the same way as mentioned above.
The parameter and result are same as mentioned above.

