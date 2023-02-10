---

title: Modeling Light Propagation
summary: We simulate photon propagation through large cortical tissue geometries in order to study the effects of scattering and develop new imaging techniques based on dynamic light scattering.

tags:
- Simulation
- Light Scattering
- Dynamic Light Scattering
- LSCI
- Multiphoton Microscopy

weight: 6

image:  
  caption: "Origin of fluorescence signal ([Davis, 2011](/publication/davis-2011/))"
  
  # Placement options: 1 = Full column width, 2 = Out-set, 3 = Screen-width
  placement: 1
    
  # Focal point options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point: Center

  # Set `preview_only` to `true` to just use the image for thumbnails
  preview_only: false

aliases:
  - /research/modeling-light-propagation

---

We study light scattering using numerical methods such as Monte Carlo or finite-difference time-domain (FDTD) simulations. These methods leverage recent advances in computational power to directly model dynamic light scattering in arbitrary three-dimensional voxelized geometries. These approaches do not require assumptions about the degree of multiple scattering or the form of the autocorrelation function and are capable of rapidly evaluating the effects of changes in particle motion. We obtain [vectorized]({{< relref "/project/vascular-vectorization" >}}) vascular geometries using [multiphoton microscopy]({{< relref "/project/multiphoton-microscopy" >}}) and assign location-appropriate optical properties. These dynamic light scattering Monte Carlo (DLS-MC) simulations have been used to understand the [depth dependence of measured fluorescence signals]({{< relref "/publication/davis-2011" >}}) and to quantify the [effects of multiple scattering events]({{< relref "/publication/davis-2015" >}}) on [laser speckle contrast imaging]({{< relref "/project/laser-speckle-contrast-imaging" >}}) (LSCI).

{{< figure src="autocorrelation.png" caption="**Calculation of autocorrelation function:** Vascular and parenchymal dynamic scattering events and autocorrelation functions simulated using DLS-MC ([Davis, 2015](/publication/davis-2015/))." >}}

We are also leveraging the versatility of DLS-MC to develop [blood flow tomography for LSCI]({{< relref "/publication/jafari-2022" >}}). This high spatial resolution computational optical imaging technique is based on the principles of LSCI and allows for reconstructing blood flow maps from speckle contrast images provided that the three-dimensional vascular structure is known or can be assumed.

{{< figure src="bloodflow.png" caption="**Reconstruction of 3D blood flow:** Volumetric illustration of ground truth and reconstructed vascular blood flow in the mouse cortex ([Jafari, 2022](/publication/jafari-2022/))." >}}
