# phone-usage
Assignment: Data analytics to group clients according to usage characteristics


Consider that you are the Information Processing Specialist for a telecommunication company. The general manager acquired your help to group the company clients based on their usage for services. The data that has the clients’ usage can be found in “Telecom” file in CuLearn.
Do the following tasks and answer the inquiries in order achieve the required grouping task.

1. As the company is planning to make promotion plans for clients based on their use for their services. Group clients based on their monthly usage for local, long distance and international calls durations by using k-means, Kohonen and two-steps clustering algorithms. For k-means and Kohonen make 5 data clusters (groups) and for the two-step algorithm keep the number of clusters (groups) between 2 and 7. The software that can be used for this assignment is SPSS Modeler.


2. Try to do the best setting possible for the algorithms to have the best clusters (groups of clients)
Ans: Settings have been uploaded as pictures

3. For each of the three clustering models, try to generate 3D model that represent the clusters. The model should have the three usage factors mentioned above (local, long distance and international calls durations); and should show each cluster with different color. Take a screenshot for each of the graphs and past them in this document. 
Ans: Solutions can be found on pictures uploaded

4. For each one of the three clustering algorithms result, explain whether it was good clustering or not with justification

I observed following properties of clusters of each of these algorithms that justify if it was good clustering or not.

#### Spatial separation between clusters

**k-means:** All clusters are spatially separated on the graph showing clear dissimilarity between heterogenous clusters. This makes it a good cluster.

**Kohonen:** I don’t think this is a good cluster. Data points are close together in x-y plane but there are also some outliers that are far away from most of other data points in their cluster. This tells me that there are no unique parameters for these clusters.
**Two-step:** 3D model shows better clustering compared to kohonen but not as good as k-means. As is observed, data points colored light blue is overlapping with data points colored dark blue. There is not enough separation between different clusters.

#### Cluster sizes

**k-means:** The ratio of sizes between largest and smallest cluster is 6.07. This plays a role in making this a good clustering algorithm as there is a wider separation is terms of size between different clusters. This tells me that there are more users that belong to one cluster than the other.
**Kohonen:** The ratio of sizes between largest and smallest cluster is 1.92. This tells me that there is not a lot of separation from one cluster size to another. This could mean that number of users that have usage characteristics described in one cluster, are similar to number of users that belong to another cluster.

**Two-step:** The ratio of sizes between largest and smallest cluster is 4.24. This ratio is high enough for me to consider it a good clustering algorithm.

#### Predictor importance

**K means:** Both long distance usage and international usage have the maximum predictor importance of “1”. This means that their usage values played in a significant role for algorithm to decide which cluster to put them in. Compared to Kohonen, where only one parameter played a role in deciding cluster, I think having two parameters play a role gives a more accurate and usable result.

**Kohonen:** Only long-distance parameter has predictor importance of 1.00. International and local have low importance, 0.18 and 0.06 respectively. This makes the algorithm weak, because it seems that international usage and local usage, while significant in k-means, are not useful for clustering in kohonen. This might make business decision biased to just the long-distance parameter.

**Two step:** All parameters have fairly high importance in deciding clusters. Long distance and international usage have importance of 1.00, while local has importance of 0.8. I believe this allows for all parameters to be represented in clusters.

#### Variation of means

**k-means:** Both long distance and international have wide variation in means for each cluster. This seems to be related to their predictor importance value. I also think that wider the difference between means of different clusters, the more heterogenous they are.

**Kohonen:** there is wide variation of means within long distance parameter (range between 1 and 25). This is the not the case with means of international (0 to 2) and local values (50 to 60) of each cluster. I consider this a drawback since for data points with boundary values for a cluster, the algorithm may not be sure which cluster to place them in.

**Two-step:** There seems to be a wide variation in means for all three parameters. In long distance usage, mean can be from range of 0. 05 to 6.99. In international usage, it varies from 3.57 to 20.57. In local from approx. 20 to 150.

5. Which clustering result do you think it was the best with justification?

To summarise, I think k-means was best clustering algorithm, followed closely behind with two step. Visually, k-means displayed better separation between dissimilar clusters. This means that it formed clusters with distinct features. It also had a cluster with highest number of data points and highest “largest to smallest” cluster size ratio. This tells me that it recognised a usage pattern that had high frequency in this data. This would give me confidence to make business decisions favoring this usage pattern. The mean usage for international, long distance and local is clearly depicted in result chart below. Additionally, wide variation in mean values of usage helps me clearly distinguish between clusters as was displayed in k-means. Sample mean values of one cluster if shown in figure

![this image](https://github.com/Vidushi187/phone-usage/blob/input-data/mean%20usage%20patterns.png)




