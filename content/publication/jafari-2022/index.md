---

title: "High-resolution three-dimensional blood flow tomography in the subdiffuse regime using laser speckle contrast imaging"
authors:
  - Chakameh Jafari
  - Samuel Mihelic
  - Shaun Engelmann
  - Andrew Dunn 
date: "2022-03-31"
doi: "10.1117/1.JBO.27.8.083011"
publication: "*Journal of Biomedical Optics*"

abstract: |
  **Significance:** Visualizing high-resolution hemodynamics in cerebral tissue over a large field of view (FOV), provides important information in studying disease states affecting the brain. Current state-of-the-art optical blood flow imaging techniques either lack spatial resolution or are too slow to provide high temporal resolution reconstruction of flow map over a large FOV.

  **Aim:** We present a high spatial resolution computational optical imaging technique based on principles of laser speckle contrast imaging (LSCI) for reconstructing the blood flow maps in complex tissue over a large FOV provided that the three-dimensional (3D) vascular structure is known or assumed.

  **Approach:** Our proposed method uses a perturbation Monte Carlo simulation of the high-resolution 3D geometry for both accurately deriving the speckle contrast forward model and calculating the Jacobian matrix used in our reconstruction algorithm to achieve high resolution. Given the convex nature of our highly nonlinear problem, we implemented a mini-batch gradient descent with an adaptive learning rate optimization method to iteratively reconstruct the blood flow map. Specifically, we implemented advanced optimization techniques combined with efficient parallelization and vectorization of the forward and derivative calculations to make reconstruction of the blood flow map feasible with reconstruction times on the order of tens of minutes.

  **Results:** We tested our reconstruction algorithm through simulation of both a flow phantom model as well as an anatomically correct murine cerebral tissue and vasculature captured via two-photon microscopy. Additionally, we performed a noise study, examining the robustness of our inverse model in presence of 0.1% and 1% additive noise. In all cases, the blood flow reconstruction error was <2% for most of the vasculature, except for the peripheral vasculature which suffered from insufficient photon sampling. Descending vasculature and deeper structures showed slightly higher sensitivity to noise compared with vasculature with a horizontal orientation at the more superficial layers. Our results show high-resolution reconstruction of the blood flow map in tissue down to 500 µm and beyond.

  **Conclusions:** We have demonstrated a high-resolution computational imaging technique for visualizing blood flow map in complex tissue over a large FOV. Once a high-resolution structural image is captured, our reconstruction algorithm only requires a few LSCI images captured through a camera to reconstruct the blood flow map computationally at a high resolution. We note that the combination of high temporal and spatial resolution of our reconstruction algorithm makes the solution well-suited for applications involving fast monitoring of flow dynamics over a large FOV, such as in functional neural imaging.
  
# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

tags:
  - LSCI
  - Dynamic Light Scattering
  - Simulation
  - Monte Carlo
  - Vectorization
  - Reconstruction

# Associated Projects (optional)
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   Publication will be listed on project page.
projects:
  - modeling-light-propagation
  - vascular-vectorization

---
