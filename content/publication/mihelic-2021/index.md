---

title: "Segmentation-Less, Automated, Vascular Vectorization"
authors:
  - Samuel Mihelic
  - William Sikora
  - Ahmed Hassan
  - Michael Williamson
  - Theresa Jones
  - Andrew Dunn
date: "2021-10-08"
doi: 10.1371/journal.pcbi.1009451
publication: "*PLOS Computational Biology*"

abstract: Recent advances in two-photon fluorescence microscopy (2PM) have allowed large scale imaging and analysis of blood vessel networks in living mice. However, extracting network graphs and vector representations for the dense capillary bed remains a bottleneck in many applications. Vascular vectorization is algorithmically difficult because blood vessels have many shapes and sizes, the samples are often unevenly illuminated, and large image volumes are required to achieve good statistical power. State-of-the-art, three-dimensional, vascular vectorization approaches often require a segmented (binary) image, relying on manual or supervised-machine annotation. Therefore, voxel-by-voxel image segmentation is biased by the human annotator or trainer. Furthermore, segmented images oftentimes require remedial morphological filtering before skeletonization or vectorization. To address these limitations, we present a vectorization method to extract vascular objects directly from unsegmented images without the need for machine learning or training. The Segmentation-Less, Automated, Vascular Vectorization (SLAVV) source code in MATLAB is openly available on GitHub. This novel method uses simple models of vascular anatomy, efficient linear filtering, and vector extraction algorithms to remove the image segmentation requirement, replacing it with manual or automated vector classification. Semi-automated SLAVV is demonstrated on three in vivo 2PM image volumes of microvascular networks (capillaries, arterioles and venules) in the mouse cortex. Vectorization performance is proven robust to the choice of plasma- or endothelial-labeled contrast, and processing costs are shown to scale with input image volume. Fully-automated SLAVV performance is evaluated on simulated 2PM images of varying quality all based on the large ($1.4\times0.9\times0.6$ mm$^3$ and $1.6\times10^8$ voxel) input image. Vascular statistics of interest (e.g. volume fraction, surface area density) calculated from automatically vectorized images show greater robustness to image quality than those calculated from intensity-thresholded images.

links:
  - name: bioRxiv
    url: https://doi.org/10.1101/2020.06.15.151076
    
# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

tags:
  - Vectorization
  - Image Processing
  - Algorithm
  - Multiphoton Microscopy
  - 2P

# Associated Projects (optional)
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   Publication will be listed on project page.
projects:
  - vascular-vectorization

---
