# Dolphin Social Network

## Overview

This project is an assignment as part of the [Data Visualization course](https://class.coursera.org/datavisualization-001). It aims to visualize a dolphins' social network and to get 
hands-on experience with the topics that are covered in the course.

[![nl-hugo/dolphins-social-network](/media/screenshot.png)](https://github.com/nl-hugo/dolphins-social-network)

This chart shows a network graph of frequent dolphin associations between 62 dolphins. The size of the node represents it's degree in the network; i.e. the larger the node, the more interactions a dolphin has with other dolphins. The color of the node represents the centrality in the network; i.e. the darker the node color, the more interactions from (sub-groups of) other dolphins go through this dolphin. This could be a measure of the importance of a dolphin in the group. Unfortunately, the data set does not contain any additional information to support such claims. The position of the nodes was determined by the Yifan Hu layout algorithm. The graph was created with [Gephi](http://gephi.github.io/).


## Source Code Layout

    data\               visualization data
    media\				media files
	LICENSE				The license file
    README.md           README file that appears on the website's github page

	
## Raw Data

The data set was downloaded as [zip-file](http://networkdata.ics.uci.edu/data/dolphins/dolphins.zip) from the University of California's Network Data Repository. It contains data about an undirected social network of frequent associations between 62 dolphins in a community living off Doubtful Sound, New Zealand.


## Data Processing

The data set was visualized using [Gephi](http://gephi.github.io/). The folling steps were taken:

1. Load dolphins.zip in Gephi

2. Run Statistics -> Network Diameter statistics to determine centrality

3. Set the node size via Nodes -> Size -> Degree 

4. Set the node color via Nodes -> Color -> Eccentricity

5. Layout the graph via Layout -> Yifan Hu