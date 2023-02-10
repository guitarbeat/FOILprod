---

title: 3D Single Particle Tracking
summary: We built a three-dimensional single particle tracking system capable of spatial localization far beyond the diffraction limit for use in studying molecular transport dynamics.

tags:
- Particle Tracking
- Multiphoton Microscopy
- 2P

weight: 9

image:  
  caption: "Internalization of single EGFR molecule ([Perillo, 2015](/publication/perillo-2015/))"
  
  # Placement options: 1 = Full column width, 2 = Out-set, 3 = Screen-width
  placement: 1
    
  # Focal point options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point: Center

  # Set `preview_only` to `true` to just use the image for thumbnails
  preview_only: false

aliases:
  - /research/3d-single-particle-tracking

---

Molecular trafficking within cells, tissues, and engineered three-dimensional (3D) multicellular models is critical to the understanding of the development and treatment of various diseases including cancer. However, current tracking methods are either confined to two dimensions or limited to depths of only 15 µm. Our aim is to develop new 3D tracking techniques and algorithms to improve tracking in tissue and *in vivo* models. We have recently developed a [new tracking method called TSUNAMI]({{< relref "/publication/perillo-2015" >}}) capable of quantifying rapid molecular transport dynamics in highly-scattering environments at depths up to 200 µm. The system has a response time of 1 ms with a temporal resolution down to 50 µs in high signal-to-noise conditions, and a spatial localization precision as good as 35 nm.

{{< figure src="TSUNAMI.png" caption="**TSUNAMI Microscope:** Schematic of the two-photon 3D tracking microscope combining nonlinear and multiplexed illumination for localization ([Perillo, 2015](/publication/perillo-2015/))." >}}

Built on spatiotemporally multiplexed [two-photon excitation]({{< relref "/project/multiphoton-microscopy" >}}), this approach requires only one detector for 3D particle tracking and allows for two-photon, multicolor imaging. An initial demonstration of the technique was performed on epidermal growth factor receptor (EGFR) complexes at a depth of 100 µm in tumor spheroids. We are currently working to extend this technique's capabilities with multi-color detection. Current application areas include early cancer diagnosis in circulating tumor cells, and study of EGFR trafficking in the cytoplasm.

{{< video src="internalization.mp4" controls="yes" caption="**Deep single-particle tracking of EGFR:** Trajectory showing internalization of single EGFR complex into 100 µm tumor spheroid ([Perillo, 2015](/publication/perillo-2015/))." >}}
