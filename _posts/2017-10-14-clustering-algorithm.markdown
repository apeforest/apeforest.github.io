---
layout: post
title:  "Clustering: Beyond K-Mean"
date:   2017-10-14 22:56:48 -0700
categories: blog
---

Clustering algorithm has been widely used in many applications.  
In VLSI design automation, clustering algorithm is used to group leaf-level gates and decide the optimal locations to insert buffers. Clustering can be based on K-mean algorithm or balanced partition algorithm depending on the objectives and often a mix of both algorithms is used. Due to the sheer number of gates (in the order of millions) hierarchical clustering algorithm is often used to form more finegrained clusters and improve overall performance such as minimal skew from siginal source to all the leaves (in the case of clock tree synthesis). In this application, clustering of gates are often deterministic, i.e. a gate is only assigned to one cluster. The distance metric is often based on eclidian distance or Manhattan distance with certain weights. 

In machine learning, the clustering models can be more general. Gaussian mixed model would form clusters in ecliptical shapes rather than circular shapes as in K-Mean. In fact, K-Mean is a special case of the Gaussian mixed model when the variance on each dimension is zero. Mixed membership model can be applied to more realworld categorization problem where an object can be assigned to multiple clusters. For example, in the case of assigning topic to articles. An article about Colin Kaepernick could be assigned to both Politics and Sports. Latent Dirchilet Allocation (LDA) method is often used to create clusters for the mixed membership model. Gibbs sampling technique is often employed to mitigate the large runtime complexity.
  
Overall, clustering is a typical unsupervised learning, not only in artificial intelligence but in our human cognitive science as well. Think about any shape in the nature. They are random in themselves. It's our human beings that gave them special meaning by performing an unsupervised learning in our mind.
