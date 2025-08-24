# numpy_depth_showcase
Method to mimic a MiDaS-style depth-from-image demo without machine learning, using transparent NumPy steps. It involves loading and normalizing an image, computing feature maps, generating a heuristic depth blend, regularizing, computing gradients, and converting the depth map into coordinate grids for 3D visualization.

## Try it out in Google Colab as primarily built here!

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RGithub23/numpy_depth_showcase/blob/main/numpy_depth_showcase.ipynb)

---

## Contents

numpy_depth_showcase.ipynb: Jupyter notebook

---

## Features

Vectorized grayscale conversion and normalization
Sobel edge magnitude via 2D convolution with numpy.lib.stride_tricks.sliding_window_view
Gaussian blur implemented in pure NumPy
A simple heuristic "depth" map blended from inverted luminance, edges, and a radial prior
Surface normals from np.gradient
A simple pinhole projection to 3D point-cloud arrays (X, Y, Z)

---
## Requirements

This Colab notebook automatically installs all necessary dependencies

## License

MIT License or your preferred license.  Attribution to Numpy for access to their open source model.

