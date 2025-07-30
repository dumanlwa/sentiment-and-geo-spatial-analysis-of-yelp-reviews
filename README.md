Project Title
Sentiment & Geo-Spatial Analysis of Yelp Reviews using Deep Learning: Uncovering Business Insights

Course
SDSC4008: Deep Learning (2024-2025 Semester B)

Project Overview
This project combines sentiment analysis and geospatial modeling on Yelp restaurant reviews to derive actionable business insights. Key objectives include:

Sentiment Classification: Predict positive/negative reviews using DNN and CNN models.

Geospatial Analysis: Identify top-performing restaurants using Graph Attention Networks (GATv2) and anomaly detection.

Business Insights: Provide data-driven recommendations for restaurant startups/expansions.

Key Components
1. Sentiment Analysis
Data Preprocessing:

Filtered English restaurant reviews.

Applied text normalization (lowercasing, stopword removal, stemming).

Feature Extraction:

Bag-of-Words model (Document-Term Matrix).

Models:

DNN: Achieved 93.58% accuracy, outperforming CNN (92.52%).

CNN: Used Conv1D layers for text classification.

Performance Metrics:

DNN: Precision = 0.95, Recall = 0.97, F1-score = 0.96 (positive class).

2. Geospatial Analysis
Graph Construction:

Nodes: Restaurants (features: longitude, latitude, log-transformed review count).

Edges: Connections to 15 nearest neighbors.

Model:

GATv2: Predicted star ratings and identified spatial outliers (top 5% anomalies).

Key Findings:

Anomalies (exceptional restaurants) average 4.6 stars (vs. 3.5 for others).

87.4% of anomalies remain open (vs. 66.9% for non-anomalies).

3. Business Insights
Top Categories for Anomalies: Sandwiches, American/Italian/Mexican cuisines.

Geographic Trends:

Urban restaurants slightly outperform rural (3.56 vs. 3.46 avg stars).

States with most anomalies: Pennsylvania, Florida, Indiana.

Review Keywords: "Friendly," "Always," "Order" suggest strategies like staff training and app-based ordering.

Conclusion
The study demonstrates how deep learning can extract practical insights from Yelp data:

DNNs excel in sentiment analysis, while GATv2 captures spatial dependencies.

Anomaly detection reveals high-performing restaurants and their traits (e.g., cuisine, location).

Actionable recommendations: Focus on popular cuisines, urban locations, and customer service.

Limitations & Future Work:

Incorporate user metadata into graph networks.

Expand analysis to non-English reviews.

References
Perez, L. (2017). Predicting Yelp star reviews using graph structures. arXiv.

Shaikh, A. H. (2019). Yelp rating classification via graph features. Dublin Business School.

