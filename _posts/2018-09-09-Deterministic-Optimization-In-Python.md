---
layout: post
title: Deterministic Optimization In Python
tags: [python, linear programming, supply chain, scheduling, PuLP]
---

<p style="text-align:justify">In this post, I explore the topic of linear programming, a very powerful deterministic optimization technique that is used for maximizing or minimizing an objective function that is constrained by a set of linear equations to form a feasible region. This post isn't going to delve into the basics of linear programming, rather, I wanted to show you how you can use Python and in specific, the PuLP modeler to formulate and solve a real-world optimization problem.</p>

<script src="https://gist.github.com/adikamath/72812b2cc1d31a9d3670ded9a723d121.js"></script>

<h3>Next Steps</h3>
<p style="text-align:justify">Now that we've formulated and solved the linear program, let's talk about how we can make this more realistic. You could explore:</p>
<ul>
<li><b>Adding changeover constraints-</b>  everytime manufacturing switches from one batch to another, there is changeover time that needs to be accounted for. During this period there is no manufacturing happening, but that time still has cost associated with it.<li>
<li><b>Insufficient Capacity-</b> Right now, we are only considering 5 day's worth of available production capacity. How can we improve the model to handle jobs that are in excess of available production capacity? Maybe we need to have roll-over days?<li>
<li><b>Jobs that arrive mid-week-</b> In our model, we've assumed a 1-week lock. Which means that any jobs that we receive throughout the week will only be scheduled for the following week starting Monday. Can we adjust the model such that it can schedule jobs that arrive mid-week in the same week?<li>
<ul>

<h2>References</h2>

<div>
<div><a href = "https://pythonhosted.org/PuLP/CaseStudies/index.html">Optimization with PuLP</a></div>
<div><a href = "https://youtu.be/5I0mhX0973o">Caylie Cincera's Videos</a></div>
<div><a href = "http://benalexkeen.com/linear-programming-with-python-and-pulp/">Ben Alex Keen's Blog</a></div>
</div>
