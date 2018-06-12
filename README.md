# kdd-cup-99-python
Analysis and preprocessing of the 10% subset of the original kdd cup 99 network intrusion detection dataset using python, scikit-learn and matplotlib.

# Testing for linear spearability

Linear separability of various attack types is tested using the Convex-Hull method. The intersections between the hull boundaries of 
the classes normal and the two most frequent attack types neptune and smurf are visualized in a 2D plot against the first two principal
components. This way it can proved that the distinct attack classes are non-linearly separable.


# Resampling using SMOTE and Cluster-Centroids

To mitigate the high class imbalance described in preprocessing well-known resampling techniques are applied to the original dataset.
Under-sampling is implemented by using the Cluster Centroids method. Hereby the data is grouped by similarity based on clustering methods with the overall goal to avoid any 
information loss as far as possible. Oversampling is based on the Synthetic Minority Oversampling Technique (SMOTE). During this technique points are randomly picked from the minority
class and synthetically enriched by appending the k-nearest neighbours to them.
