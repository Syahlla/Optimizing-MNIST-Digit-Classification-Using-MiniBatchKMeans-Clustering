### Summary

**Methodology:**

1. **Data Import and Preprocessing:**
   - Imported the MNIST dataset using Keras.
   - Split the data into training and testing sets.
   - Reshaped and normalized the data for further processing.

2. **Data Visualization:**
   - Visualized the first 36 samples of the training set with their labels.

3. **Clustering:**
   - Applied MiniBatchKMeans clustering algorithm.
   - Determined the optimal number of clusters by evaluating models with different cluster counts (300, 400, 500, 1000).
   - Calculated evaluation metrics: inertia, homogeneity, and accuracy for each cluster configuration.
   - Inferred cluster labels based on the most frequent label in each cluster.

4. **Cluster Optimization:**
   - Identified the optimal number of clusters (1000) with the highest homogeneity and accuracy.
   - Visualized the centroids of the first 26 clusters.

**Results:**

- **Optimal Number of Clusters:**
  - 1000 clusters were identified as the optimal number, resulting in high homogeneity (0.8997) and accuracy (0.9301).

- **Cluster Quality:**
  - Inertia for the optimal cluster configuration was 1,259,562.60, indicating tight clustering.
  - Visualization of the cluster centroids showed clear, distinguishable digits, validating the effectiveness of the clustering.

- **Accuracy:**
  - The final accuracy of the model was 93.01%, showing that the clustering algorithm correctly grouped similar digits together with high precision.

### Conclusion

Using the MiniBatchKMeans clustering algorithm on the MNIST dataset, the study achieved high-quality clustering with 1000 clusters. The model demonstrated high accuracy and homogeneity, confirming the suitability of the chosen approach for effectively clustering handwritten digit images.
