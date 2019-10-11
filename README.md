# Commercial centers using POI

[![Build Status](https://travis-ci.org/pages-themes/cayman.svg?branch=master)](https://travis-ci.org/pages-themes/cayman) [![Gem Version](https://badge.fury.io/rb/jekyll-theme-cayman.svg)](https://badge.fury.io/rb/jekyll-theme-cayman)


Identify commercial centers using Points of Interest (POI) data by clustering these points into commercial centers/markets.

## Getting Started

How to use
```    
git clone git@github.com:aakashjhawar/commercial-centers-using-POI.git
cd commercial-centers-using-POI
jupyter notebook
```
Start the jupyter server. The following should be executed in order.
*   gather-data.ipynb
*   DBSCAN-remove-noise.ipynb
*   create-clusters.ipynb

---

#### 1. gather-data.ipynb
It uses Overpy (Python wrapper for Overpass) to gather all the nodes of a particular location and stores the data into a csv.
It also cleans the dataset based on amenities.

#### 2. DBSCAN-remove-noise.ipynb
It removes the noise/outliers present in the dataset. It also gives the number of clusters that can be formed from the dataset.

#### 3. create-clusters.ipynb
It uses KMeans Clustering to create clusters and plot them on Google Map using gmplot library.

Check out the [Github repo page](https://aakashjhawar.github.io/commercial-centers-using-POI/)
