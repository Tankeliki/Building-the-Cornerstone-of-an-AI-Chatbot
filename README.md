# Building-the-Cornerstone-of-an-AI-Chatbot
This project was developed as part of a hackathon, focusing on clustering and analyzing text data to build the foundation for an AI-powered chatbot. By using Natural Language Processing (NLP) and unsupervised machine learning techniques, the objective is to categorize text data into meaningful clusters, which can help train the chatbot to respond more effectively based on the input it receives. The K-Means clustering algorithm is used to group customer support queries into different topics.

# Key Features
Text Preprocessing: Cleans and transforms raw text data into a numerical format using Term Frequency-Inverse Document Frequency (TF-IDF) vectorization.
Cluster Selection: Uses the Elbow Method and Silhouette Score to determine the optimal number of clusters for the data.
K-Means Clustering: Applies K-Means clustering to categorize documents based on the number of clusters chosen.
Cluster Analysis: Extracts the top words for each cluster to interpret the themes or topics in each group.
PCA Visualization: Reduces data dimensions to 2D and visualizes clusters to help interpret the clustering results.

# Prerequisites
```bash
pip install pandas numpy re nltk torch seaborn matplotlib scikit-learn
```

# Overview of Functions
```
1. Preprocess Text
Converts raw text into numerical format using TF-IDF.
Scales the data to normalize the features.
2. Visualize Cluster Selection
Uses the Elbow Method and Silhouette Score to help determine the optimal number of clusters (k).
3. Train K-Means
Trains a K-Means clustering model with a chosen number of clusters.
4. Extract Top Words per Cluster
Identifies the most significant words in each cluster for better interpretability.
5. Visualize Clusters
Uses Principal Component Analysis (PCA) to reduce the data to 2D and visualizes the clusters.
6. Clustering Pipeline
Orchestrates the entire clustering process:
Preprocessing the data.
Generating cluster selection plots.
Training K-Means and extracting cluster keywords.
Visualizing the clusters.
```

# Instructions to Run the Pipeline
-Prepare a list of documents (e.g., customer queries, FAQs, etc.) for clustering.
-Call the clustering_pipeline(documents) function where documents is the list of raw text data.
-The system will:
  Preprocess the text and scale the features.
  Display plots for the Elbow Method and Silhouette Score to assist in selecting the optimal number of clusters (k).
  Ask the user to input the best number of clusters based on the graphs.
  Train the K-Means model with the chosen number of clusters.
  Display the top words that represent each cluster.
  Visualize the clusters in a 2D plot using PCA.

#Conclusion
This project demonstrates how text clustering can be used to create a valuable AI tool, such as a chatbot. The K-Means algorithm, combined with text preprocessing and visualization techniques, helps identify common topics in customer support queries, enabling the chatbot to learn from these clusters and respond accordingly.

  
