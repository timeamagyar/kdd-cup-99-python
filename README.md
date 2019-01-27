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

## Licensing 

Copyright (c) 2019, Timea Magyar
All rights reserved.
 
Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

Redistributions of source code must retain the above copyright notice, this
list of conditions and the following disclaimer.

Redistributions in binary form must reproduce the above copyright notice,
this list of conditions and the following disclaimer in the documentation
and/or other materials provided with the distribution

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
