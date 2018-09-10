---
layout: post
title: Dijkstra's Algorithm In Python
tags: [python, algorithms, supply chain]
---

<p style="text-align:justify">This short post is going to be about my take on implementing Dijkstra's Algorithm in Python. In my quest to learn about more tools in the Supply Chain Analytics toolkit, I've been taking this online course offered by MIT's Centre For Logistics And Transportation. This is where I was first introduced to this algorithm. It's often used to find the shortest distance between any two nodes in a network.

Let's use an example to describe a problem and also to code it- you own a trucking company and you transport goods to your customers in 13 cities. The list of cities which also form the nodes in your network have been coded as S, A, B, C, D, E, F, G, H, I, J, K and L. The graph for this is shown below:</p>

<img src= "/assets/img/dijkstras.png">

<p style="text-align:justify">You want to find the shortest distance between city 'S' and city 'E' and also which exact cities to visit on your way to the destination. In order to use Dijkstra's Algorithm to solve this problem, here are the steps you would need to follow:</p>

<ol>
<li>Get the list of all cities and their weights or distances from each other.
</li>
<li>Create a network(graph) that represents the connections between these nodes.
</li>
<li>Select a source node and an ending node. Set the source node as the current node.
</li>
<li>For each node in the network except the source node, assign the distance from the source node to it to infinity.
</li>
<li>Make sure to track all nodes that you have visited. A node is considered as visited once we have calculated the distance from itself to all other nodes that are connected to it (also called its neighbors).
</li>
<li>Set the values of all distances to nodes/cities from the source node as 0.
</li>
<li>For the current node, consider all of its neighbors and for each, calculate the distance to the current node from source node and sum it to the distance from the current node to the distance under consideration. If this value is less than the current value for the node, then change the nodes value to the value you just calculated. Once all the nodes neighbors are considered, mark the node as visited.
</li>
<li>Select the next unvisited node with the smallest distance from the source and set it as the current node and follow the same procedure until you select the next current node.
</li>
<li>Once the end node has been selected, the algorithm is complete.
</li>
<li>The shortest distance is the weight of the ending node and the shortest path is the order in which you have stored nodes in your visited nodes set.
</li>
</ol>

<p>Let's code this!</p>

<script src="https://gist.github.com/adikamath/04f021169eb3e7784b1f8554814fe61b.js"></script>

<h2>References</h2>
<p style="text-align:justify">Over the course of developing my own implementation of the Dijkstra's Algorithm, I scoured the internet for articles and references. Here are the posts that helped me the most:</p>

<div>
<div><a href = "https://www.youtube.com/watch?v=GazC3A4OQTE&t=112s">Dijkstra's Algorithm- Computerphile</a></div>
<div><a href = "https://www.geeksforgeeks.org/greedy-algorithms-set-6-dijkstras-shortest-path-algorithm/">Greedy Algorithms</a></div>
</div>
<p> </p>
