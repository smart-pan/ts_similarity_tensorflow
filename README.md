# Similarity measures for time series implemented in tensorflow.
### 1. Soft-Dynamic Time Warping (SDTW).
  - File: [SoftDTW.py](https://github.com/PeteWe/ts_similarity_tensorflow/blob/master/SoftDTWTF.py)
  - Notes: Inputs of shape: (n,t,f).
    - n: number of multivariate time series.
    - t: length of time series.
    - f: number of features.
  - Source: [Cuturi, Blondel (2017) - Soft-DTW: a Differentiable Loss Function for Time-Series](https://arxiv.org/pdf/1703.01541.pdf)
### 2. Complexity-Invariant Distance (CID).
  - File: [CIDTF.py](https://github.com/PeteWe/ts_similarity_tensorflow/blob/master/CIDTF.py)
  - Notes: Inputs of shape: (n,t,1)...currently implemented for univariate time series only. Multivariate implementation might follow.
    - n: number of multivariate time series.
    - t: length of time series.
  - Source: [Batista et al. (2011) - A Complexity-Invariant Distance Measure for Time Series](http://www.cs.ucr.edu/~eamonn/Complexity-Invariant%20Distance%20Measure.pdf)
### 3. Euclidean distance (ED).
  - File: [EDTF.py](https://github.com/PeteWe/ts_similarity_tensorflow/blob/master/EDTF.py)
  - Notes: Inputs of shape: (n,t,f).
    - n: number of multivariate time series.
    - t: length of time series.
    - f: number of features.
  - Borrowed from: [Guo et al. (2017) - Improved Deep Embedded Clustering with Local Structure Preservation](https://github.com/XifengGuo/IDE)
