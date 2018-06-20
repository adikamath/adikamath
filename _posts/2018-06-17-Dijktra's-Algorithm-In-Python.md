---
layout: post
title: Dijkstra's Algorithm In Python
tags: [python, algorithms, supply chain]
---

<p style="text-align:justify">This short post is going to be about my take on implementing Dijkstra's Algorithm in Python. In my quest to learn about more tools in the Supply Chain Analytics toolkit, I've been taking this online course offered by MIT's Centre For Logistics And Transportation. This is where I was first introduced to this algorithm. It's often used to find the shortest distance between any two nodes in a network.

Let's use an example to describe a problem and also to code it- you own a trucking company and you transport goods to your customers in 13 cities. The list of cities which also form the nodes in your network have been coded as S, A, B, C, D, E, F, G, H, I, J, K and L. The graph for this is shown below:</p>

<img src= "/Users/adityakamath/Documents/adikamath.github.io/assets/img/dijkstras.png">

<p style="text-align:justify">You want to find the shortest distance between city 'S' and city 'E' and also which exact cities to visit on your way to the destination. In order to use Dijkstra's Algorithm to solve this problem, here are the steps you would need to follow:

1.  Get the list of all cities and their weights or distances from each other.
2.  Create a network(graph) that represents the conections between these nodes.
3.  Select a source node and an ending node. Set the source node as the current node.
4.  For each node in the network except the source node, assign the distance from the source node to it to infinity.
5.  Make sure to track all nodes that you have visited. A node is considered as visited once we have calculated the       distance from itself to all other nodes that are connected to it (also called its neighbors).
6.  Set the values of all distances to nodes/cities from the source node as 0.
7.  For the current node, consider all of its neighbors and for each, calculate the distance to the current node from     source node and sum it to the distance from the current node to the distance under consideration. If this value       is less than the current value for the node, then change the nodes value to the value you just calculated. Once       all the nodes neighbors are considered, mark the node as visited.
8.  Select the next unvisited node with the smallest distance from the source and set it as the current node and           follow the same procedure until you select the next current node.
9.  Once the end node has been selected, the algorithm is complete.
10. The shortest distance is the weight of the ending node and the shortest path is the order in which you have stored     nodes in your visited nodes set.

Let's code this!</p>
