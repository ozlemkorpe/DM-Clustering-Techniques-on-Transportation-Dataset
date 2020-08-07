# DM-Clustering-Techniques-on-Transportation-Dataset
Data mining project applied on Antalya bus dataset.

![Complete Workflow](https://github.com/ozlemkorpe/DM-Clustering-Techniques-on-Transportation-Dataset/blob/master/screenshots/complete-workflow.png)

This project was built using [Knime](https://www.knime.com/).

## Columns
- **Linename**: Name of the bus line. 
- **Lineid**: Unique ID's of lines.
- **Route**: Name of the bus route.
- **Routeid**: ID of the bus route. Each route has unique ID.
- **Stopname**: Name of the bus stop.
- **Stopid**: Unique ID of bus stop.
- **StopSequence**: Visit sequence of the bus for each stop.

## Usage
All files are excluded from Knime environment, they must be opened by using Knime. Necessary dataset can also be found in the Dataset folder and destination of the dataset must be reconfigured in file reader node.

## Grouping Operations
GroupBy node is used for grouping bus routes with count of bus stops it passing by, finding possible bus stations by grouping bus stops by its stop sequences, finding most and least used bus stops.

## Similarity Search
String distances are calculated for line and stopnames by using String Distances node and aggregated by using Aggregated Distance node. By using Similarity Search node, similar row analyzed.

## Clustering Techniques
Clustering techniques are used for clustering bus routes with its similarity. Bus routes which passing by more common bus stops are accepted as similar.

### K-Means Clustering
![K-Means Clustering Results](https://github.com/ozlemkorpe/DM-Clustering-Techniques-on-Transportation-Dataset/blob/master/screenshots/kmeans.png)

### DB-Scan Clustering
![DBScan Clustering Results](https://github.com/ozlemkorpe/DM-Clustering-Techniques-on-Transportation-Dataset/blob/master/screenshots/dbscan.png)

### Hierarchical Clustering
![Hierarchical Clustering Results](https://github.com/ozlemkorpe/DM-Clustering-Techniques-on-Transportation-Dataset/blob/master/screenshots/hierarchical.png)

## Performance Evaluation
![Time Performances](https://github.com/ozlemkorpe/DM-Clustering-Techniques-on-Transportation-Dataset/blob/master/screenshots/performancetime.png)
## Map Viewer


## Authors
* **Özlem Körpe** - *Initial work* - [ozlemkorpe](https://github.com/ozlemkorpe)
