# Coursera_Capstone

## Overview

Capstone project - Exploring restaurants in Los Angeles and predicting optimal locations for new restaurant setups. Uses Folium for producing maps indicating venue locations. For the learning part, I use a K-means clustering for segmenting the various neighborhoods according to restaurant densities and types.

## Technical Details

The grave details of the project are all mentioned in the [notebook](https://github.com/jyotisman-ds/Coursera_Capstone/blob/main/Exploring LA Restaurants.ipynb)

- Location data was obtained from  [here](https://usc.data.socrata.com/dataset/Los-Angeles-Neighborhood-Map/r8qd-yxsr)

- The number of neighborhoods was truncated to 199 using a distance function from the LA central coordinates.

- Two ideas are explored here in detail. One idea is to find the density of restaurants in each neighborhood. This will help anyone trying to open a new restaurant by either avoiding overcrowded areas or alternately could also help finding popular venues for someone looking to avoid competition. The above data also includes the area of each neighborhood in square miles which can be used to compute this density I mentioned. A K-Means clustering technique is then used to segment neighborhoods based on this data.

- Second idea is to explore the kind of restaurants. Here, one can again use clustering but now based on the frequency of occurrence of each restaurant in a neighborhood. Once we find the relevant cluster here, we can then look for its intersection with the clusters found above to fine tune the relevant neighborhood where one wants to open his/her restaurant. A snippet of such a final cluster with all the information included is shown below -

![cluster1](/images/cluster_1.png)

- Figure shows the Cluster labelled as '1'. It plots the number of restaurants in each category from the most common restaurant venues list. On top of that, it also shows how many of them are in low, medium and high density neighborhoods.

## Use cases

I prepared a small [presentation](https://github.com/jyotisman-ds/Coursera_Capstone/blob/main/presentations/Final_project_presentation.pdf) to pitch this idea in a commercial setting with an example as well. Do check it out!

# Credits
A huge shoutout to the Coursera community for hosting the IBM professional certificate [course](https://www.coursera.org/professional-certificates/ibm-data-science) and to all the instructors of this course.
