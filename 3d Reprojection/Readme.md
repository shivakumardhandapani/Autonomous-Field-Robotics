# 3D Reconstruction with Structure-from-Motion using GTSAM

This notebook implements a full **Structure-from-Motion (SfM)** pipeline for 3D reconstruction from 2D images using key computer vision and optimization techniques. It leverages **SIFT-based feature extraction**, **RANSAC filtering**, and **GTSAM** for bundle adjustment and graph-based optimization. The final result is a reconstructed sparse 3D point cloud of a scene from a multi-view image dataset.

## 📌 Project Highlights

- Extracted keypoints and descriptors using **SIFT**
- Matched features across consecutive images using **BFMatcher**
- Filtered noisy correspondences using **RANSAC**
- Estimated relative camera poses and triangulated 3D points
- Constructed and optimized a factor graph using **GTSAM**
- Visualized the resulting 3D point cloud using **Open3D**

## 🛠️ Technologies & Libraries

- Python 3
- OpenCV (SIFT, RANSAC)
- NumPy, SciPy
- GTSAM (`gtbook`)
- Open3D
- Google Colab
- Matplotlib, Plotly (for visualization)

## 📊 Results

- Sparse 3D point cloud reconstructed from a sequence of static images
- Optimized camera pose graph
- Interactive 3D visualizations of the reconstructed scene

## 📎 Notes

- The current implementation uses **grayscale images** for feature detection.
- Camera intrinsics are assumed to be known and fixed (defined via matrix `K`).
- Bundle adjustment via **GTSAM** significantly improves reconstruction accuracy.

---
