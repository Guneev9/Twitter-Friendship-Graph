# Twitter-Friendship-Graph

An example of a Friendship graph and further their communities.

## Input:
A user with more than 10,000 followers

##  Friendship Graph:

Crawl Function():
1) Start with user with more than 10,000 followers

2)Fetch its reciprocal friends

3)Then, from step-2 get its Top-5 reciprocal friends using the above get_user_profile() function

4)Append these to the csv file in order to create ege list

5)Then repeat the steps 2-4 till distance-3 so that we get atleast 100 nodes for graph

This will give followers.csv file which will be used to plot the community detection graph

## Community Detection:
Community detection using Norman-Girvan Algorithm based on edge-betweeneness.

Algorithm:(Divisive Hierarchical Clustering)

1)It detects communities by progressively removing edges from the original graph
2)It will removes the “most valuable” edge, that is the edge with the highest betweenness centrality, at each step.
3)As the graph breaks down into pieces, the tightly knit community structure is exposed

It is upto user that, till what depth, you want to break. I have break down the graph into communities till 
level-4(divisive clustering)
