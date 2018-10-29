---
layout: post
title: Exploring Clustering Algorithms Using Scikit-learn
tags: [python, machine learning, supply chain, scikit-learn]
---

<p style="text-align:justify">In this post we're going to look at applying a class of simple unsupervised machine learning algorithms called clustering. Specifically we're going to be looking at two types of clustering apporaches called Hierarchical Agglomerative Clustering and K-Means Clustering using the Scikit-learn framework in Python. The dataset that we're going to analyze contains demand data for a large number of Part Numbers belonging to several product families. The intent is to see how we can use the nature of the demand as a feature to help us create product families.</p>

<img src= "/assets/img/clustering_pics.png">

<script src="https://gist.github.com/adikamath/9e1052d9511235237f773635c8bddd97.js"></script>

<h3>What's Next?</h3>
<p style="text-align:justify">We've reached the end of this blog post having explored two clustering approaches in trying to solve a supply chain business case. In the process, we performed some data wrangling and preprocessing to prepare the data for clustering and also briefly looked at different ways of improving the clustering results. This analysis is by no means complete and you could explore different evaluation methods to see how effective the clusters that we've created are. The clusters are nothing but product families and the next step in the analysis pipleine might be forecasting demand for these families. So a natural question that arises is how does the type of clustering algorithm affect the 'forecastability' of your product families? Let me know what you think!</p>

<h2>References</h2>
<div>
<div><a href = "http://benalexkeen.com/feature-scaling-with-scikit-learn/">Ben Alex Keen On Feature Scaling</a></div>
<div><a href = "https://towardsdatascience.com/the-5-clustering-algorithms-data-scientists-need-to-know-a36d136ef68">George Seif On Clustering</a></div>
<div><a href = "https://www.youtube.com/watch?v=ikt0sny_ImY">K-Means Clustering</a></div>
<div><a href = "https://stackabuse.com/hierarchical-clustering-with-python-and-scikit-learn/">Hierarchical Agglomerative Clustering</a></div> 
</div>
<p></p>