# first-clustring-project

# About Dataset(information from https://archive.ics.uci.edu/ml/datasets/Query+Analytics+Workloads+Dataset):
The data-set contains three (3) sets of synthetic range and radius query workloads derived from Gaussian distributions over the real dataset in [URL-1]. Each processed query is associated with aggregate scalar values (count, sum, average) over the dataset in [URL-1].

[URL-1]: [Web Link]

Note: the current dataset is processed data derived after synthetic query analytics workloads over the real-dataset in [URL-1] and does not include any data from [URL-1].

Attribute Information:

[*] The dataset 'Radius Queries' contains records of the format: {'X-coordinate','Y-coordinate', 'R-Radius'}. These queries define a disc over a 2D space with center (X,Y) and radius R in order to investigate the number of crime incidents, the total arrests and the average beat of the disc region (spatial area) defined by each query.

[*] The dataset 'Radius Queries Count' contains records of the format: {'X-coordinate','Y-coordinate', 'R-Radius', 'Count'}. These queries define a disc over a 2D space with center (X,Y) and radius R and the number of crime incidents Count of the disc region (spatial area) defined by each query.

[*] The dataset 'Range Queries Aggregates' contains records of the format: {'X-coordinate','Y-coordinate', 'X-range', 'Y-range', 'Count', 'SUM', 'AVG'}.
These queries define a rectangle over a 2D space with coordinates/points: X +/- X-range and Y +/- Y-range. The count, sum, and avg is the number of incidents, total arrests and average beat of the rectangle region (spatial area) defined by each query.

[*] All datasets are .csv

Example of a Range Query with Count, SUM, and AVG:

[1159191.2534425869,1894755.9479944962,5225.375665408865,2981.728430851036,96046.0,34927.0,1111.618901359765]

where:
'X-coordinate' = 1159191.2534425869,
'Y-coordinate' = 1894755.9479944962,
'X-range' = 5225.375665408865,
'Y-range' = 2981.728430851036,
'Count' = 96046.0,
'SUM' = 34927,
'AVG' = 1111.618901359765.

Attribute Information:

Attributes:
'ID' = serial number of query (optional)
'X-coordinate' = spatial x-coordinate (float)
'Y-coordinate' = spatial y-coordinate (float)
'R-Radius' = spatial radius of a disc (X,Y) for radius query (float)
'X-range' = spatial x-range for range query (float)
'Y-range' = spatial y-range for range query (float)
'Count' = number of crime incidents in the 2D disc (radius queries) or rectangle (range queries)
'SUM' = summation of Arrests in the 2D disc (radius queries) or rectangle (range queries)
'AVG' = average Beat in the 2D disc (radius queries) or rectangle (range queries)


# About Project:
In this project i used the first 2 dataset of this Datasets and i used sckit-learn package for preprocessing data and  kmeans and for hierarcy i used scipy package.for the first dataset(Radius Queries) i used Kmeans and for knowing the number of clusters  i used elbow method and found that the number of clusters is 4.

In the second dataset(Radius-Queries-Count) i used hierarchy and for knowing the number of clusters i used Dendogram plot and found that 3 clusters.
